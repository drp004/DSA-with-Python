# Space & Time Complexity

Before we dive into Data Structures and Algorithms, we need to understand the fundamental language of algorithmic efficiency: Space and Time Complexity.

When writing code, there are usually dozens of ways to solve the same problem. But how do we know which solution is the "best"? We evaluate them based on how much time they take to run and how much memory (space) they consume as the input size grows.

---

### What is Big O Notation?

Big O Notation is the mathematical metric we use to describe the efficiency of an algorithm. It focuses on the worst-case scenario, answering the question: "As our input data (n) grows infinitely large, how does our algorithm perform?"

---

### ⏱️ Time Complexity

Time complexity is not about measuring the exact execution time in seconds (since that depends on your hardware). Instead, it measures the number of operations an algorithm performs relative to the input size.

Time Complexity tells us: How the running time of an algorithm grows as the input size increases.


#### Common Time Complexities:

1. O(1) - Constant Time: 
The execution time remains the exact same, regardless of the input size.

2. O(log n) - Logarithmic Time:
The execution time increases incredibly slowly as the input grows. The algorithm typically halves the data set with each iteration.

3. O(n) - Linear Time:
The execution time grows directly in proportion to the input size. If the input is 10 times larger, it takes 10 times longer.

4. O(n log n) - Linearithmic Time:
Common in efficient sorting algorithms like Merge Sort and Quick Sort. It performs an O(n) operation for each O(log n) split of the data.

5. O(n^2) - Quadratic Time:
The execution time is proportional to the square of the input size. This usually happens with nested loops and becomes very slow with large inputs.

---

### 💾 Space Complexity

Space complexity measures the total amount of memory an algorithm requires to run as a function of the input size.

Note: Total Space Complexity = Auxiliary Space (extra space used by the algorithm) + Space used by the input. Usually, when we say "Space Complexity" in interviews, we are referring to the Auxiliary Space.

#### Common Space Complexities:

1. O(1) - Constant Space:
The algorithm uses a fixed amount of extra memory, regardless of the input size.

2. O(n) - Linear Space:
The extra memory used grows in proportion to the input size. This usually happens when you create a new data structure (like a list or hash map) based on the input.

---

### 🛠️ Rules for Calculating Complexity
To easily identify the complexity of your Python code, follow these three simple rules:

1. Worst Case Usually Dictates Big O: If a loop might stop early if it finds a value, we still assume the worst-case scenario where the value is at the very end.

2. Drop Constants: O(3n) becomes O(n). O(n/2) becomes O(n).

3. Drop Non-Dominant Terms: O(n^2 + n + 5) becomes O(n^2) because n^2 grows much faster and dominates the memory/time footprint as n gets larger.

---