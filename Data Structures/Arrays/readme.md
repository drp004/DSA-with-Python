# Arrays in Python

Welcome to the Arrays section! Arrays are one of the simplest and most widely used data structures. In Python, the array data structure is implemented as the built-in list.Arrays are used to build other data structures like Stack Queue, Deque, Graph, Hash Table, etc

---

### Definition:

An array is a linear data structure that stores a fixed-size sequence of elements of the same data type in contiguous memory locations. Each element can be accessed directly using its index, which allows for efficient retrieval and modification.

Example: arr = [10, 20, 30, 40, 50]

Here:
- Index starts from 0
- arr[0] = 10
- arr[2] = 30

--- 

### Space & Time Complexity:

#### Space Complexity: O(n) 

- An array of n elements takes O(n) space.


#### Time complexities:

1. Access element by index: O(1)

2. Insert element at end: O(1)

3. Insert element at middle: O(n)

4. Delete element: O(n)

5. Searching:     
    - unsorted: O(n) (linear search)
    - sorted: O(log n) (binary search)

---

#### Types of Arrays:

1D Array:
```
arr = [1, 2, 3]
```

2D Array (Matrix):
```
matrix = [
 [1, 2],
 [3, 4]
]
```

---

#### Advantages of Array:

1. Fast access (O(1))
2. Cache-friendly (contiguous memory)
3. Simple and easy to use
4. Efficient for fixed-size data
5. Supports binary search (if sorted)

---

#### Disadvantages of Array:

1. Fixed size (static arrays)
2. Insertion/deletion is slow (O(n))
3. Memory wastage if size is large but unused
4. Requires contiguous memory block
5. Not suitable for frequent modifications

---

### Static vs. Dynamic Arrays


#### Static Arrays: 

Have a fixed size defined when they are created (common in languages like C++ or Java). If you run out of room, you have to create a brand new, larger array and copy everything over manually.


#### Dynamic Arrays (Python Lists): 

Automatically resize themselves when they run out of space. Under the hood, when a Python list gets full, it automatically allocates a new chunk of contiguous memory (usually double the size) and moves the existing elements there.

---

#### When to Use Array?

- You need fast random access
- Data size is fixed or rarely changes
- Frequent read operations
- Working with:
    - Matrices
    - Lookup tables
    - Sliding window problems
    - Binary search problems


#### When NOT to Use Array?

- Frequent insertions/deletions
- Size changes often
- Memory is fragmented

In such cases → `Linked List` is better.

---
