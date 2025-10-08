# Experiment 16 

## Name: Gandluri Sai Tejas
## Class: ENTC A2
## PRN.:24070123045
## Title: Implementation of Recursion in C++
---

## Aim
To study and implement recursion in C++ by writing programs for:  
1. Calculating factorial of a number.  
2. Finding the sum of first `n` natural numbers.  
3. Reversing a string using recursion.  

---

## Objectives
- To understand the concept of recursion and its applications in problem-solving.  
- To implement recursive functions for mathematical and string operations.  
- To compare recursion with iteration in terms of simplicity, readability, and efficiency.  
- To observe how function calls are managed using the **call stack** during recursion.  

---
   

## Theory

Recursion is a fundamental concept in computer science and mathematics. In programming, **recursion is a technique where a function calls itself** in order to solve a larger problem by breaking it into smaller, similar sub-problems. 
It is based on the principle of **"Divide and Conquer"**, where each recursive call works on a smaller portion of the problem until a **base case** is reached, after which the calls start returning results back up the chain (called **unwinding of recursion**).

---

### 1. Working of Recursion
When a recursive function is called:
1. **Function Call Created** – Each invocation of the function is pushed onto the call stack.
2. **Check for Base Case** – If the base condition is true, recursion stops.
3. **Recursive Call Execution** – If the base case is false, the function calls itself with a modified input.
4. **Unwinding** – When the base case is met, values are returned back step by step until the original function call is resolved.

For example:  
Factorial(5) → 5 × Factorial(4) → 5 × 4 × Factorial(3) → … → 5 × 4 × 3 × 2 × 1.  

---

### 2. Key Components of Recursion
- **Base Case:** Prevents infinite recursion by defining when the recursion should stop.  
- **Recursive Case:** Defines the part of the function where recursion occurs.  
- **Call Stack:** Recursion uses system memory to store each active function call until the base case is reached.  

---

### 3. Advantages of Recursion
- **Simplifies complex problems** like tree traversal, backtracking, and divide-and-conquer algorithms (Merge Sort, Quick Sort).  
- **Closer to mathematical formulations** (factorial, Fibonacci, GCD).  
- **Improves readability** by reducing code length for repetitive problems.  

---

### 4. Disadvantages of Recursion
- **Memory intensive**: Each function call consumes stack memory. Deep recursion may cause **stack overflow error**.  
- **Performance overhead**: Recursive calls are slower due to repeated function invocations compared to iteration.  
- **Debugging difficulty**: Tracing recursive calls can be harder for beginners.  

---

### 5. Real-life Examples of Recursion
- **Mathematics:** Factorials, Fibonacci series, exponentiation.  
- **Data Structures:** Traversal of trees and graphs (DFS).  
- **Sorting Algorithms:** Quick sort, Merge sort, Heap sort.  
- **Searching Algorithms:** Binary search (recursive form).  
- **Backtracking Problems:** Sudoku solver, N-Queens problem, maze solving.  
- **System Applications:** Directory and file system traversal, compiler parsing.  

---

### 6. Types of Recursion
1. **Direct Recursion:** Function directly calls itself.  
   Example: `factorial(n)` calls `factorial(n-1)`.  
2. **Indirect Recursion:** A function calls another function, which in turn calls the first one.  
3. **Tail Recursion:** Recursive call is the last statement in the function. Compiler can optimize tail recursion to reduce memory usage.  
4. **Non-Tail Recursion:** Recursive call is followed by other operations (e.g., multiplication in factorial).  

---

### 7. Recursion vs Iteration
Both recursion and iteration are used to solve repetitive problems, but they differ in how they achieve repetition.

| Feature              | Recursion                          | Iteration                     |
|-----------------------|------------------------------------|-------------------------------|
| Definition            | Function calling itself            | Loop repeats until condition  |
| Base/Termination      | Requires a base case               | Requires loop condition       |
| Memory Usage          | High (uses call stack)             | Low (no stack calls)          |
| Performance           | Slower due to function overhead    | Faster due to direct looping  |
| Code Readability      | More elegant, compact              | More verbose, longer          |
| Risk                  | Stack overflow                     | Infinite loop                 |
| Applications          | Trees, graphs, divide & conquer    | Simple counting, summation    |

---
### Real-life applications include:

Mathematical computations (factorial, Fibonacci).

Data structures (trees, graphs).

Backtracking problems (N-Queens, Sudoku).

Algorithm design (divide and conquer).

Hence, recursion is a powerful concept that enhances problem-solving ability in C++ programming.

# Programs and algorithms
### 1. Factorial
1. Start program.  
2. Input number `n`.  
3. If `n == 0` or `n == 1`, return 1 (base case).  
4. Else, return `n * factorial(n-1)` (recursive case).  
5. Print result.  
6. End.

### 2. Sum of N Natural Numbers
1. Start program.  
2. Input number `n`.  
3. If `n == 0`, return 0 (base case).  
4. Else, return `n + sum(n-1)` (recursive case).  
5. Print result.  
6. End.

### 3. String Reversal
1. Start program.  
2. Input string.  
3. If `start >= end`, return (base case).  
4. Swap `str[start]` with `str[end]`.  
5. Call function recursively with `start+1` and `end-1`.  
6. Print reversed string.  
7. End.

---


## Program Summary
- Implemented three recursive programs: factorial, sum of natural numbers, and string reversal.  
- Demonstrated **base case** and **recursive case** in each program.  
- Showed how recursion simplifies code for problems involving repetitive breakdown.  

---

## Concepts Used
- **Recursion** (self-calling functions).  
- **Functions in C++** for modularity.  
- **Control Structures** (`if-else` conditions).  
- **Call Stack Mechanism** (stack frames in recursion).  
- **String Handling** (manual length calculation and character swapping).  

---

## Conclusion
This experiment demonstrated the concept and implementation of recursion in C++.  

We observed that:  
- Recursion simplifies code for problems like factorial, summation, and string reversal.  
- **Base case** is essential to avoid infinite recursion.  
- Compared to iteration, recursion uses more memory but provides cleaner and more mathematical solutions.
- 
Hence, recursion is a powerful concept that enhances problem-solving ability in C++ programming.  
