# Linear Data Structure

## Array

```
length: n。
query：O（1）
insert：O（n）
delete：O（n）
```

## LinkedList

```
length: n。
query：O（n）
insert && delete：O（1）
```

### Applications

- Stack, Queue, binary trees, and graphs are implemented using linked lists.
- Dynamic management for Operating System memory.
- Forward and backward operation in the browser.

## Stack

```
length: n
query：O（n）
insert && delete：O（1）
```

### Applications

- Redo and Undo operations in doc editors
- Reversing a string
- Function calls order

## Queue

```
length: n
query：O（n）
insert && delete：O（1）
empty：front == rear
full：（rear+1）% maxsiz == front
```

### Single Queue

### Circular Queue

### Applications

- Breadth-first search algorithm in graphs
- Operating system: job scheduling operations, Disk scheduling, CPU scheduling etc.
- Call management in call centres

### Deque

### Priority Queue
