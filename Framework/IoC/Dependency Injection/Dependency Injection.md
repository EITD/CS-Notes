# Dependency Injection

1. Without dependency injection
    - We creates a dependency between the `Client` and the `ExamplieService`.
        
        We are instantiating `ExamplieService` every time we call `Client()`, which means the `Client` class directly depends on the `ExamplieService` class.
        
    
    ```java
    public class Client {
    
    private ExampleService service;
    
        Client() {
            service =new ExampleService();
        }
    }
    ```
    
2. Constructor Injection
    
    We create an abstraction by having the `ExamplieService` dependency class in `Client`'s constructor signature (not initializing dependency in class). 
    
    ```java
    public class Client {
    
    private ExampleService service;
    
        Client(Service service) {
            this.service = service;
        }
    }
    ```
    
    - This allows us to call the dependency then pass it to the `Client` class like so:
        
        ```java
        ExampleService service = new ExampleService(); // dependency
        Client client = new Client(service);
        ```
        
3. Setter Injection
    
    ```java
    public void setService(Service service) {
    		this.service = service;
    }
    ```
    
4. Interface Injection
    
    ```java
    public interface ServiceSetter {
    		public void setService(Service service);
    }
    
    public class Client implements ServiceSetter {
    		private Service service;
    
    		@Override
    		public void setService(Service service) {
    				this.service = service;
        }
    }
    ```