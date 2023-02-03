# Linear Data Structure

## Array

```
假如数组的长度为 n。
访问：O（1）
插入：O（n）
删除：O（n）
```

## LinkedList

```
假如链表中有n个元素。
访问：O（n）
插入删除：O（1）
```

### Applications

- Stack, Queue, binary trees, and graphs are implemented using linked lists.
- Dynamic management for Operating System memory.
- Forward and backward operation in the browser.

## Stack

```
假设堆栈中有n个元素。
访问：O（n）
插入删除：O（1）
```

### Applications

- Redo and Undo operations in doc editors
- Reversing a string
- Function calls order

## Queue

```
假设队列中有n个元素。
访问：O（n）
插入删除：O（1）
队列为空：front == rear
队列为满：（rear+1）% maxsiz == front
（少用一个存储空间，数组的最后一个存数空间不用）
```

### Single Queue

### Circular Queue

### Applications

- Breadth-first search algorithm in graphs
- Operating system: job scheduling operations, Disk scheduling, CPU scheduling etc.
- Call management in call centres

### Deque

### Priority Queue