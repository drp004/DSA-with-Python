## Queue

A queue is a linear data structure that follows the `First In, First Out (FIFO)` principle, where the first element added to the queue is the first one to be removed.

Elements in a queue are added to the end (`rear`) and removed from the beginning (`front`).

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20250827110558739481/Dequeue-Operation-in-Queue-1.webp">

#### Real-life examples:

- People standing in a line
- Ticket counter
- Printer queue

---

### Basic Operations:

```
Operation	    Meaning                             Time            Space      
                                                    complexity      complexity
enqueue(x)	    Insert element at the rear          O(1)            O(1)
dequeue()	    Remove element from the front       O(1)            O(1)
peek()	        View front element                  O(1)            O(1)
isFull()	    Check if queue is full              O(1)            O(1)
isEmpty()	    Check if queue is empty             O(1)            O(1)
```

---

### Time & Space Complexity

#### Time complexity:

- In Queue insertion only happens on front and removal only happens on rear, beacause of this time complexity is `O(1)`.

#### Space Complexity: 

- A queue storing n elements takes `O(n)` space.

---

### Queue implementation

1. Array/List
2. Linked List
3. collection.queue     (for python)
4. collection.deque     (for python)

---

### Types of Queue

#### 1. Simple Queue:

- Which follows simple `FILO` structure.

#### 2. Circular Queue:

- Circular Queue is a linear data structure in which the operations are performed based on `FIFO` principle and the last position is connected back to the first position to make a circle.

- This queue is primarily used in the following cases:
    - Memory Management
    - Traffic system
    - CPU Scheduling

#### 3. Input restricted Queue:

- In this type of Queue, the input can be taken from one side only(`rear`) and deletion of elements can be done from both sides(`front` and `rear`).

- This queue is used in cases where the consumption of the data needs to be in FIFO order but if there is a need to remove the recently inserted data for some reason and one such case can be irrelevant data, performance issue, etc. 

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20220623131417/inputrestrictedqueue.jpg">

#### 4. Output restricted Queue:

- In this type of Queue, the input can be taken from both sides(`rear` and `front`) and the deletion of the element can be done from only one side(`front`).

- This queue is used in the case where the inputs have some priority order to be executed and the input can be placed even in the first place so that it is executed first.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20220623131455/outputrestrictedqueue.jpg">

#### 5. Double ended Queue (`Deque`):

- Double Ended Queue is also a Queue data structure in which the insertion and deletion operations are performed at both the ends (`front` and `rear`).

- Since Deque supports both stack and queue operations, it can be used as both.

- The Deque data structure supports clockwise and anticlockwise rotations in `O(1)` time which can be useful in certain applications.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20220623131811/doubleended.jpg">

#### 6. Priority Queue:

- A priority queue is a special type of queue in which each element is associated with a priority and is served according to its priority.

- There are two types of Priority Queues:

    1. `Ascending Priority Queue`: Element can be inserted arbitrarily but only smallest element can be removed.

    2. `Descending priority Queue`: Element can be inserted arbitrarily but only the largest element can be removed first from the given Queue.

---

### Advantages of Queue:

1. All operations are `O(1)`
2. Maintains processing order
3. Useful for scheduling tasks
4. Dynamic size (linked list / deque)
5. Simple and efficient
 
---

### Disadvantages:

1. No random access (can’t access middle directly)
2. Searching takes `O(n)`
3. Array implementation may waste space (if not circular)

---

When to Use Queue?

- First-come-first-serve processing
- Order preservation
- Level-wise processing

---