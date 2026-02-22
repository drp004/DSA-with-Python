## Stacks in Python

A Stack is a linear data structure that operates on a very specific rule: LIFO (Last In, First Out). 

This means that the last element added is the first one to be removed. In a stack, both insertion and deletion happen at the same end, which is called the top of the stack.


#### Real-life example:

- Stack of plates, Last plate placed → removed first

---

### Basic Operations

A stack supports mainly 4 operations:
```
Operation	    Meaning                         Time            Space
                                                complexity      complexity
push(x)	        Insert element at top           O(1)            O(1)
pop()	        Remove top element              O(1)            O(1)
peek()/top()	Returns the topmost element     O(1)            O(1)
isFull()        Check if stack is full          O(1)            O(1)
isEmpty()	    Check if stack is empty         O(1)            O(1)
```

---

### ⏱️ Time & Space Complexity:

#### Time complexity:

Because a stack restricts where you can add and remove data, its core operations are incredibly fast.

#### Space complexity:

If stack has n elements: Space = O(n)

Because:

- Stores n elements, No extra structure

---

### Stack implementation:

Stacks can be implemented using:

1. Using Arrays/List

2. Using Linked List (when dynamic size needed)

---

### Advantages of Stack:

1. All operations are O(1)

2. Simple and fast

3. Useful for tracking order

4. Memory efficient

5. Supports recursion internally

---

### Disadvantages:

1. Access only top element (restricted access)

2. Cannot search efficiently (O(n))

3. Possible overflow (fixed-size array stack)

---

### When to Use Stack:

- Reverse order processing

- Last-in-first-out behavior

- Tracking previous states

---