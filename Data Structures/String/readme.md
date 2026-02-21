## Strings in Python

Welcome to the Strings section! At a basic level, strings are just sequences (or arrays) of characters. Many of the techniques you learned in the Arrays section will apply directly here.

However, strings in Python have one massive difference from lists that you must understand to write efficient algorithms: Immutability.

So internally: String = Character Array

Example: 
```
s = "hello"
```

Memory view:
```
Index	Character
  0	        h
  1	        e
  2	        l
  3	        l
  4	        o
```

---

### 🧠 How Strings Work: The Immutability Rule

Like arrays, strings are stored in contiguous memory locations. You can access any character instantly if you know its index.

But unlike Arrays / lists, strings are immutable. This means once a string is created in memory, it cannot be changed.

If you try to modify a string (for example, adding a character to the end or changing a specific letter), Python doesn't just change the existing string. Instead, it:

1. Allocates brand new memory for the new string.

2. Copies all characters from the old string into the new memory space.

3. Adds the new character(s).

Building a string by repeatedly adding characters in a loop using `+=` will secretly cost you a lot of time and memory.

--- 

### String operations:

- `Concatenation`: operation of joining two or more character strings end-to-end to create a new, combined string. 

    Python uses the `+` operator (e.g., a + b), or `s.join()` for joining multiple strings.

- `Substring` A substring is a contiguous sequence of characters within a larger string. 

    Uses slicing with square brackets [] and indices. 

    Example: 
    ```
    s = "python" 
    print(s[0:2])    # result: py
    ```

As string is `Immutable`, changes in string creates new string each time.

---

### ⏱️ Time & Space Complexity

#### Space Complexity: O(n)

#### Time complexities:

1. Access character by index: O(1)

2. Concatenate: O(n + m)

3. Searching: O(n)

4. Slicing: O(k)

5. Length: O(1)

---

### Advantages of String

1. Fast access (O(1))

2. Contiguous memory (cache friendly)

3. Easy manipulation

4. Safe (immutable in Python/Java)

5. Useful for text processing

---

### Disadvantages

1. Immutable → extra memory usage

2. Concatenation is expensive

3. Frequent modification is slow

4. Not suitable when many updates are needed

For heavy modifications use:

- List + join (Python)

- StringBuilder (Java)

---
