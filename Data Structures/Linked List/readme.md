## Linked List

A Linked List is a linear data structure where elements are stored in nodes, and each node contains:
- `Data`
- `Reference` (pointer) to the next node

The first node is called the `head` node and we can traverse the whole list using this `head` and `next` links.

`Null`/`None` indicates end of list.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20250619155958124670/Linked-list.webp">

A linked list is a fundamental data structure in computer science. It mainly allows efficient insertion and deletion operations compared to arrays. 

Like arrays, it is also used to implement other data structures like stack, queue and deque.

--- 

### Types Of Linked Lists:

#### 1. Singly Linked List:

Singly linked list is the simplest type of linked list in which every node contains some data and a pointer to the next node of the same data type. 

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20240917161540/Singly-Linked-List.webp">

#### 2. Doubly Linked List:

A doubly linked list or a two-way linked list is a more complex type of linked list that contains a pointer to the next as well as the previous node in sequence. 

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20240917161540/Doubly-Linked-List.webp">

#### 3. Circular Linked List:

A circular linked list is a type of linked list in which the last node's next pointer points back to the first node of the list, creating a circular structure. This design allows for continuous traversal of the list, as there is no null to end the list.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20240917161541/Circular-Linked-List.webp">

---

### Basic Operations

```
Operation                       Time Complexity

Insert at beginning                 O(1)
Insert at middle / end              O(n)
Delete at beginning                 O(1)
Delete at middle / end              O(n)
Search / Access by index            O(n)
Traversal                           O(n)
```

---

### Time & Space Complexity

#### Time complexity:

For most of the operations we have to traverse linked list node by node because of that most of the operations have time complexity as `O(n)`.

#### Space omplexity:

If list has n nodes: Space = `O(n)`

But each node also stores:
- Data
- Pointer

So memory overhead is higher than array.

---

### Advantages of Linked List:

1. Dynamic size (no fixed capacity)
2. Efficient insertion/deletion (`O(1)` at head)
3. No memory wastage due to pre-allocation
4. Works well when size changes frequently
5. No need for contiguous memory

---

### Disadvantages:

1. No random access (`O(n)`)
2. Extra memory for pointers
3. Slower than arrays (poor cache locality)
4. More complex implementation

---

### When to Use Linked List?

- Frequent insertions/deletions
- Size is unknown or changing
- Memory is fragmented
- Implementing:
    - Stack (linked version)
    - Queue
    - Hash chaining
    - Graph adjacency list

---