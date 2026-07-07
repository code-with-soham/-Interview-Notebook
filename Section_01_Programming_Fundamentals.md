# ═══════════════════════════════════════════════════════

# SECTION 1: PROGRAMMING FUNDAMENTALS

# ═══════════════════════════════════════════════════════

---

## 1.1 C++ Fundamentals

### ✅ Important Topics

- [ ] Data types, type casting, type conversion
- [ ] Input/Output streams
- [ ] Control flow (if, else, switch, loops)
- [ ] Functions (pass by value, pass by reference, default arguments)
- [ ] Inline functions
- [ ] Function overloading
- [ ] Scope resolution operator
- [ ] Namespace
- [ ] const keyword (const variables, const pointers, const member functions)
- [ ] static keyword (static variables, static functions, static members)
- [ ] volatile keyword
- [ ] typedef and using
- [ ] enum and enum class
- [ ] Preprocessor directives (#define, #include, #ifdef, #pragma)
- [ ] Command line arguments
- [ ] Lambda expressions
- [ ] auto keyword
- [ ] Range-based for loop
- [ ] nullptr vs NULL

### 📋 Interview Questions

1. What is the difference between C and C++?
2. What are the features of C++ that make it different from C?
3. Explain the compilation process of a C++ program.
4. What is the difference between `#include <iostream>` and `#include "iostream"`?
5. What is the difference between `endl` and `\n`?
6. What is the difference between `cin` and `getline()`?
7. What is the difference between `struct` and `class` in C++?
8. What is the difference between `new` and `malloc()`?
9. What is the difference between `delete` and `free()`?
10. Explain implicit and explicit type conversion in C++.
11. What is the use of the `const` keyword in C++? Give all use cases.
12. What is the use of the `static` keyword in C++? Give all use cases.
13. What are inline functions? When should you use them?
14. What are lambda expressions in C++? Give syntax and example use case.
15. What is the difference between `typedef` and `using`?

### 🔥 Frequently Asked Questions

16. What is the difference between `++i` and `i++`?
17. What is the size of different data types in C++?
18. What happens when you divide an integer by zero in C++?
19. What is the difference between `float` and `double`?
20. Explain the difference between `break`, `continue`, and `return`.
21. What is the ternary operator?
22. What are storage classes in C++?
23. What is the difference between local and global variables?

---

## 1.2 Pointers

### ✅ Important Topics

- [ ] Pointer declaration and initialization
- [ ] Pointer arithmetic
- [ ] Null pointer
- [ ] Dangling pointer
- [ ] Wild pointer
- [ ] Void pointer
- [ ] Pointer to pointer
- [ ] Pointer to array
- [ ] Array of pointers
- [ ] Function pointers
- [ ] Pointer to function
- [ ] this pointer
- [ ] Smart pointers (unique_ptr, shared_ptr, weak_ptr)
- [ ] Dynamic memory allocation (new, delete, new[], delete[])
- [ ] Memory leak

### 📋 Interview Questions

1. What is a pointer? How do you declare and initialize it?
2. What is the difference between a pointer and a reference?
3. What is a null pointer? How is it different from a dangling pointer?
4. What is a wild pointer?
5. What is a void pointer? When is it used?
6. What is pointer arithmetic? What operations are valid on pointers?
7. What is a pointer to a pointer? Give a real-world use case.
8. What are function pointers? Where are they used?
9. What is the `this` pointer in C++?
10. What are smart pointers? Why were they introduced?
11. What is the difference between `unique_ptr`, `shared_ptr`, and `weak_ptr`?
12. What is a memory leak? How do you prevent it?
13. What is the difference between stack and heap memory allocation?
14. What happens if you `delete` a pointer twice?
15. What is the difference between `new/delete` and `malloc/free`?

### 🎯 Scenario Based Questions

16. Given a dangling pointer bug in code, how would you identify and fix it?
17. When would you prefer `shared_ptr` over `unique_ptr`?
18. How would you implement a simple memory pool using pointers?
19. You have a function that returns a pointer to a local variable. What happens?
20. How does pointer aliasing affect compiler optimization?

---

## 1.3 Memory Management

### ✅ Important Topics

- [ ] Stack vs Heap
- [ ] Static memory allocation
- [ ] Dynamic memory allocation
- [ ] Memory layout of a C++ program (Code, Data, BSS, Stack, Heap)
- [ ] Memory fragmentation
- [ ] Memory alignment
- [ ] RAII (Resource Acquisition Is Initialization)
- [ ] Copy semantics vs Move semantics
- [ ] lvalue vs rvalue
- [ ] Move constructor and Move assignment
- [ ] Perfect forwarding

### 📋 Interview Questions

1. Explain the memory layout of a C++ program.
2. What is the difference between stack and heap memory?
3. What is RAII? Why is it important?
4. What is the difference between deep copy and shallow copy?
5. What are lvalue and rvalue in C++?
6. What is move semantics? Why was it introduced in C++11?
7. What is the difference between copy constructor and move constructor?
8. What is `std::move()`? What does it actually do?
9. What is perfect forwarding?
10. What is memory fragmentation? How do you avoid it?
11. When is stack memory preferred over heap memory?
12. What happens when the stack overflows?
13. How does `sizeof` work? What does `sizeof` a pointer return?

---

## 1.4 References

### ✅ Important Topics

- [ ] Reference declaration
- [ ] Reference vs Pointer
- [ ] lvalue reference
- [ ] rvalue reference
- [ ] const reference
- [ ] Pass by reference
- [ ] Return by reference
- [ ] Reference collapsing

### 📋 Interview Questions

1. What is a reference in C++?
2. What is the difference between a reference and a pointer?
3. Can a reference be null?
4. Can you reassign a reference?
5. What is a const reference? Why is it useful?
6. What is the difference between pass by value, pass by reference, and pass by pointer?
7. What is an rvalue reference? When was it introduced?
8. What is reference collapsing?
9. When should you return by reference?
10. What happens if you return a reference to a local variable?

---

## 1.5 Object-Oriented Programming (OOP)

### ✅ Important Topics

- [ ] Classes and Objects
- [ ] Access specifiers (public, private, protected)
- [ ] Constructors (default, parameterized, copy, move)
- [ ] Destructor
- [ ] Encapsulation
- [ ] Abstraction
- [ ] Inheritance (single, multiple, multilevel, hierarchical, hybrid)
- [ ] Polymorphism (compile-time and runtime)
- [ ] Function overloading
- [ ] Operator overloading
- [ ] Function overriding
- [ ] Virtual functions
- [ ] Pure virtual functions
- [ ] Abstract class
- [ ] Interface
- [ ] Friend function and friend class
- [ ] Static members
- [ ] Mutable keyword
- [ ] Diamond problem
- [ ] Virtual inheritance
- [ ] Object slicing
- [ ] SOLID principles
- [ ] Composition vs Inheritance
- [ ] Aggregation vs Association
- [ ] Design patterns (Singleton, Factory, Observer, Strategy)

### 📋 Interview Questions

1. What are the four pillars of OOP?
2. What is encapsulation? Give a real-world example.
3. What is abstraction? How is it different from encapsulation?
4. What is inheritance? What are the types of inheritance in C++?
5. What is polymorphism? Explain compile-time and runtime polymorphism.
6. What is the difference between function overloading and function overriding?
7. What is a virtual function? Why is it needed?
8. What is a pure virtual function?
9. What is an abstract class? Can you create an object of an abstract class?
10. What is the diamond problem? How do you solve it?
11. What is virtual inheritance?
12. What is object slicing?
13. What is a friend function? Is it a violation of encapsulation?
14. What is operator overloading? Which operators cannot be overloaded?
15. What is the difference between a shallow copy and a deep copy?
16. When is a copy constructor called?
17. What is the Rule of Three? What is the Rule of Five?
18. What is the difference between a constructor and a destructor?
19. Can a constructor be virtual? Why or why not?
20. Can a destructor be virtual? When should it be?
21. What are access specifiers? Explain each.
22. What is the order of constructor and destructor calls in inheritance?
23. What is a static member variable? How is it different from a regular member?
24. What is a static member function?
25. Can you access private members of a class from outside? How?

### 🔥 Frequently Asked Questions

26. Explain SOLID principles with examples.
27. What is the difference between composition and inheritance? When would you prefer one over the other?
28. What is the Singleton design pattern? How do you implement it in C++?
29. What is the Factory design pattern?
30. What is the Observer design pattern?
31. What is the difference between an interface and an abstract class?
32. Can you have a constructor in an abstract class?
33. What is multiple inheritance? What problems can it cause?
34. What is the difference between aggregation and composition?
35. What is the Liskov Substitution Principle? Give an example of its violation.

### 🎯 Scenario Based Questions

36. Design a class hierarchy for a vehicle management system.
37. How would you implement a notification system using the Observer pattern?
38. You need to ensure only one database connection exists. Which pattern would you use?
39. How would you design a payment processing system that supports multiple payment methods?
40. You have a base class pointer pointing to a derived class object. What happens when you call a non-virtual function?

---

## 1.6 STL (Standard Template Library)

### ✅ Important Topics

- [ ] Vectors
- [ ] List
- [ ] Deque
- [ ] Stack
- [ ] Queue
- [ ] Priority Queue
- [ ] Map
- [ ] Unordered Map
- [ ] Set
- [ ] Unordered Set
- [ ] Multimap
- [ ] Multiset
- [ ] Pair
- [ ] Tuple
- [ ] Iterators
- [ ] Algorithms (sort, find, binary_search, lower_bound, upper_bound, accumulate, etc.)
- [ ] Comparators
- [ ] Functors

### 📋 Interview Questions

1. What is STL? What are its components?
2. What is the difference between `vector` and `array`?
3. What is the time complexity of `push_back()` in a vector?
4. How does a vector grow internally?
5. What is the difference between `size()` and `capacity()` of a vector?
6. What is the difference between `map` and `unordered_map`?
7. What is the internal implementation of `map`?
8. What is the internal implementation of `unordered_map`?
9. What is the difference between `set` and `unordered_set`?
10. What is the difference between `map` and `multimap`?
11. What is the time complexity of insertion, deletion, and search in `map` vs `unordered_map`?
12. What is a priority queue? What is its internal implementation?
13. How do you create a min-heap using `priority_queue`?
14. What is the difference between `list` and `vector`?
15. What is a deque? How is it different from a vector?
16. What are iterators? What types of iterators exist?
17. What is the difference between `begin()` and `rbegin()`?
18. How do you sort a vector in descending order?
19. What is a comparator? How do you write a custom comparator?
20. What is a functor?
21. What is the difference between `lower_bound()` and `upper_bound()`?
22. What is `emplace_back()` and how is it different from `push_back()`?
23. What is the difference between `erase()` and `remove()` for vectors?

---

## 1.7 Templates

### ✅ Important Topics

- [ ] Function templates
- [ ] Class templates
- [ ] Template specialization
- [ ] Variadic templates
- [ ] Template metaprogramming basics
- [ ] Type traits

### 📋 Interview Questions

1. What are templates in C++? Why are they used?
2. What is the difference between function templates and class templates?
3. What is template specialization?
4. What is partial template specialization?
5. What are variadic templates?
6. Can a template have a default argument?
7. What is SFINAE?
8. What is the difference between templates and macros?

---

## 1.8 Time Complexity & Space Complexity

### ✅ Important Topics

- [ ] Big O notation
- [ ] Big Omega notation
- [ ] Big Theta notation
- [ ] Best, Average, and Worst case analysis
- [ ] Amortized analysis
- [ ] Time complexity of common operations
- [ ] Space complexity analysis
- [ ] Auxiliary space vs Total space
- [ ] Recurrence relations
- [ ] Master theorem

### 📋 Interview Questions

1. What is time complexity? Why is it important?
2. Explain Big O, Big Omega, and Big Theta notations.
3. What is the difference between best case, average case, and worst case?
4. What is amortized time complexity? Give an example.
5. What is the time complexity of accessing an element in an array? In a linked list?
6. What is the time complexity of insertion in a BST? In a balanced BST?
7. Compare O(1), O(log n), O(n), O(n log n), O(n²), O(2ⁿ), O(n!) in order.
8. What is the space complexity of a recursive function?
9. What is auxiliary space?
10. What is the Master Theorem? When can it be applied?
11. What is the time complexity of merging two sorted arrays?
12. If a loop runs n/2 times, what is its time complexity?
13. What is the time complexity of nested loops?
14. How do you calculate the time complexity of a recursive function using recurrence relations?

### 💻 Practical Coding Questions

15. Find the time complexity of: `for(i=1; i<=n; i=i*2)`
16. Find the time complexity of: `for(i=n; i>=1; i=i/2)`
17. Find the time complexity of: nested loops where inner loop depends on outer loop variable.
18. Find the time complexity of: `for(i=0; i<n; i++) for(j=0; j<n; j++) for(k=0; k<n; k++)`
19. Find the time complexity of: `T(n) = T(n-1) + n`
20. Find the time complexity of: `T(n) = 2T(n/2) + n`

---

## 1.9 Recursion

### ✅ Important Topics

- [ ] Base case and recursive case
- [ ] Head recursion vs Tail recursion
- [ ] Multiple recursion
- [ ] Recursion vs Iteration
- [ ] Stack overflow in recursion
- [ ] Memoization
- [ ] Recursive tree visualization
- [ ] Recursion with backtracking

### 📋 Interview Questions

1. What is recursion? What are its advantages and disadvantages?
2. What is the difference between direct and indirect recursion?
3. What is tail recursion? Why is it more efficient?
4. What is the difference between recursion and iteration?
5. What causes stack overflow in recursion? How do you prevent it?
6. What is memoization? How does it optimize recursion?
7. How do you convert a recursive function to an iterative one?

### 💻 Practical Coding Questions

8. Write a recursive function to calculate factorial of n.
9. Write a recursive function for Fibonacci series.
10. Print all subsequences of a string using recursion.
11. Tower of Hanoi — solve for n disks.
12. Write a recursive function to reverse a string.
13. Write a recursive function to check if a string is a palindrome.
14. Calculate power(x, n) using recursion (optimize to O(log n)).
15. Find the sum of digits of a number using recursion.
16. Print all permutations of a string.
17. Generate all subsets of a given set.
18. Count the number of ways to climb n stairs (1 or 2 steps at a time).
19. Recursive function to find GCD of two numbers.
20. Merge sort implementation using recursion.
21. Quick sort implementation using recursion.
22. Flatten a nested array using recursion.

---

## 1.10 Backtracking

### ✅ Important Topics

- [ ] Backtracking template/pattern
- [ ] Pruning
- [ ] State space tree
- [ ] Constraint satisfaction
- [ ] Permutations and Combinations
- [ ] N-Queens
- [ ] Sudoku Solver
- [ ] Rat in a Maze
- [ ] Word Search
- [ ] Subset Sum

### 📋 Interview Questions

1. What is backtracking? How is it different from brute force?
2. What is pruning in backtracking?
3. What is the time complexity of a backtracking algorithm?
4. When should you use backtracking?

### 💻 Practical Coding Questions

5. Solve the N-Queens problem.
6. Solve a Sudoku puzzle using backtracking.
7. Rat in a Maze — find all paths from top-left to bottom-right.
8. Generate all permutations of an array.
9. Generate all subsets (power set).
10. Word Search — find if a word exists in a 2D grid.
11. Combination Sum — find all combinations that sum to a target.
12. Generate all valid parentheses for n pairs.
13. Letter combinations of a phone number.
14. Palindrome partitioning of a string.
15. M-Coloring problem on a graph.
16. Knight's tour problem.
17. Subset sum problem.
18. Print all paths from source to destination in a graph.

---

## 1.11 Searching Algorithms

### ✅ Important Topics

- [ ] Linear Search
- [ ] Binary Search
- [ ] Binary Search on answer
- [ ] Ternary Search
- [ ] Search in rotated sorted array
- [ ] Search in 2D matrix
- [ ] Exponential Search
- [ ] Interpolation Search

### 📋 Interview Questions

1. What is the time complexity of linear search?
2. What is binary search? What are its prerequisites?
3. What is the time complexity of binary search?
4. What is the difference between iterative and recursive binary search?
5. When would you use linear search over binary search?

### 💻 Practical Coding Questions

6. Implement binary search (iterative and recursive).
7. Find the first and last occurrence of an element in a sorted array.
8. Find the square root of a number using binary search.
9. Search in a rotated sorted array.
10. Find peak element in an array.
11. Search in a 2D sorted matrix.
12. Find minimum in a rotated sorted array.
13. Find the Kth smallest/largest element.
14. Allocate minimum number of pages (binary search on answer).
15. Aggressive cows problem.
16. Find the median of two sorted arrays.
17. Count occurrences of a number in a sorted array.
18. Find the element that appears once in a sorted array (all others appear twice).

---

## 1.12 Sorting Algorithms

### ✅ Important Topics

- [ ] Bubble Sort
- [ ] Selection Sort
- [ ] Insertion Sort
- [ ] Merge Sort
- [ ] Quick Sort
- [ ] Heap Sort
- [ ] Counting Sort
- [ ] Radix Sort
- [ ] Bucket Sort
- [ ] Stability of sorting algorithms
- [ ] In-place vs Not in-place
- [ ] Comparison-based vs Non-comparison-based sorting

### 📋 Interview Questions

1. What is the difference between stable and unstable sorting?
2. What is in-place sorting?
3. Compare all sorting algorithms by time and space complexity.
4. Which sorting algorithm is best for nearly sorted data? Why?
5. Which sorting algorithm is best for linked lists? Why?
6. Why is Quick Sort preferred over Merge Sort for arrays?
7. Why is Merge Sort preferred over Quick Sort for linked lists?
8. What is the worst case of Quick Sort? How do you avoid it?
9. What is the lower bound of comparison-based sorting?
10. When would you use Counting Sort over Quick Sort?

### 💻 Practical Coding Questions

11. Implement Bubble Sort and optimize it.
12. Implement Selection Sort.
13. Implement Insertion Sort.
14. Implement Merge Sort.
15. Implement Quick Sort with different pivot strategies.
16. Implement Heap Sort.
17. Implement Counting Sort.
18. Sort an array of 0s, 1s, and 2s (Dutch National Flag).
19. Sort an array based on frequency of elements.
20. Merge two sorted arrays without extra space.
21. Sort a nearly sorted (K-sorted) array.
22. Find the minimum number of swaps to sort an array.

---

## 1.13 Bit Manipulation

### ✅ Important Topics

- [ ] AND, OR, XOR, NOT, Left Shift, Right Shift
- [ ] Check if a number is odd or even using bits
- [ ] Check, Set, Clear, Toggle a bit
- [ ] Count set bits
- [ ] Power of 2 check
- [ ] XOR properties
- [ ] Bit masking
- [ ] Brian Kernighan's algorithm

### 📋 Interview Questions

1. What are bitwise operators in C++?
2. What is the difference between `&` and `&&`?
3. What is the difference between `<<` and `>>`?
4. What is XOR? What are its important properties?
5. How do you check if a number is a power of 2 using bit manipulation?

### 💻 Practical Coding Questions

6. Check if the ith bit is set or not.
7. Set the ith bit of a number.
8. Clear the ith bit of a number.
9. Toggle the ith bit.
10. Count the number of set bits in a number (Brian Kernighan's algorithm).
11. Find the only non-repeating element in an array where every other element appears twice.
12. Find two non-repeating elements in an array where every other element appears twice.
13. Find the element that appears once when every other appears three times.
14. Swap two numbers without using a temporary variable.
15. Find the missing number in an array of 1 to n.
16. Reverse bits of a number.
17. Check if a number is a power of 2.
18. Find the position of the rightmost set bit.
19. Generate all subsets using bitmask.
20. XOR of all numbers from 1 to n.

---

## 1.14 Strings

### ✅ Important Topics

- [ ] String basics (char array vs string class)
- [ ] String manipulation methods
- [ ] Palindrome
- [ ] Anagram
- [ ] Substring
- [ ] Subsequence
- [ ] String matching algorithms (Naive, KMP, Rabin-Karp)
- [ ] Trie-based string operations
- [ ] String hashing

### 📋 Interview Questions

1. What is the difference between `char[]` and `string` in C++?
2. What is the difference between a substring and a subsequence?
3. What is the KMP algorithm? What problem does it solve?
4. What is the time complexity of the KMP algorithm?
5. What is Rabin-Karp algorithm?

### 💻 Practical Coding Questions

6. Reverse a string.
7. Check if a string is a palindrome.
8. Check if two strings are anagrams.
9. Find the longest palindromic substring.
10. Find the longest common subsequence.
11. Implement strstr() / find first occurrence of a substring.
12. Count and say problem.
13. Longest substring without repeating characters.
14. Group anagrams.
15. Minimum window substring.
16. Valid parentheses.
17. Longest common prefix.
18. String to integer (atoi).
19. Roman to integer and integer to Roman.
20. Rabin-Karp string matching.
21. Implement KMP algorithm.
22. Find all permutations of a string.
23. Smallest window containing all characters of another string.
24. Check if a string is a valid palindrome (ignoring non-alphanumeric characters).
25. Longest repeating character replacement.

---

## 1.15 Arrays

### ✅ Important Topics

- [ ] Array basics
- [ ] Subarrays, Subsequences, Subsets
- [ ] Prefix sum
- [ ] Kadane's algorithm
- [ ] Two pointers technique
- [ ] Sliding window
- [ ] Dutch National Flag algorithm
- [ ] Moore's Voting algorithm
- [ ] Matrix operations
- [ ] Spiral traversal

### 📋 Interview Questions

1. What is the difference between an array and a linked list?
2. What is the time complexity of insertion and deletion in an array?
3. What is the difference between a subarray and a subsequence?
4. What is a prefix sum array? Where is it used?

### 💻 Practical Coding Questions

5. Find the largest element in an array.
6. Find the second largest element without sorting.
7. Check if an array is sorted.
8. Remove duplicates from a sorted array (in-place).
9. Rotate an array by K positions (left and right).
10. Move all zeros to the end.
11. Find the union and intersection of two sorted arrays.
12. Find the missing number in an array of 1 to n.
13. Maximum subarray sum (Kadane's algorithm).
14. Maximum product subarray.
15. Find the longest subarray with sum K.
16. Find the majority element (Moore's Voting Algorithm).
17. Find the leaders in an array.
18. Find the stock buy and sell problem (max profit).
19. Trapping rainwater problem.
20. Container with most water.
21. Next permutation.
22. Set matrix zeros.
23. Rotate a matrix by 90 degrees.
24. Spiral traversal of a matrix.
25. Pascal's Triangle.
26. Find the duplicate number (Floyd's algorithm).
27. Merge overlapping intervals.
28. Find all pairs with a given sum.
29. Find the subarray with given XOR.
30. Longest consecutive sequence.
31. Three sum problem.
32. Four sum problem.
33. Find the repeating and missing number.
34. Count inversions in an array.
35. Reverse pairs.

---

## 1.16 Linked List

### ✅ Important Topics

- [ ] Singly Linked List
- [ ] Doubly Linked List
- [ ] Circular Linked List
- [ ] Floyd's Cycle Detection
- [ ] Merge Sort on Linked List
- [ ] Reverse a Linked List
- [ ] Intersection of two Linked Lists
- [ ] LRU Cache

### 📋 Interview Questions

1. What is a linked list? What are its types?
2. What are the advantages and disadvantages of a linked list over an array?
3. What is Floyd's Cycle Detection algorithm?
4. What is the time complexity of insertion/deletion in a linked list vs array?

### 💻 Practical Coding Questions

5. Reverse a singly linked list (iterative and recursive).
6. Detect a cycle in a linked list.
7. Find the starting node of a cycle.
8. Find the middle of a linked list.
9. Merge two sorted linked lists.
10. Remove the nth node from the end.
11. Add two numbers represented as linked lists.
12. Check if a linked list is a palindrome.
13. Find the intersection point of two linked lists.
14. Sort a linked list using Merge Sort.
15. Flatten a multilevel linked list.
16. Reverse nodes in K groups.
17. Clone a linked list with random pointers.
18. Rotate a linked list by K positions.
19. Delete a node without head pointer.
20. Implement LRU Cache.
21. Remove duplicates from a sorted linked list.
22. Remove duplicates from an unsorted linked list.
23. Odd-Even linked list segregation.

---

## 1.17 Stack

### ✅ Important Topics

- [ ] Stack operations (push, pop, peek, isEmpty)
- [ ] Implementation using array and linked list
- [ ] Monotonic stack
- [ ] Next Greater Element pattern
- [ ] Stack using queues
- [ ] Expression evaluation
- [ ] Parentheses matching

### 📋 Interview Questions

1. What is a stack? What are its applications?
2. What is the difference between stack and queue?
3. What is a monotonic stack? Where is it used?
4. How can you implement a stack using two queues?

### 💻 Practical Coding Questions

5. Implement a stack using arrays.
6. Implement a stack using linked list.
7. Implement a stack using two queues.
8. Valid parentheses.
9. Next greater element.
10. Next smaller element.
11. Previous greater element.
12. Previous smaller element.
13. Largest rectangle in histogram.
14. Maximal rectangle in a binary matrix.
15. Min stack (O(1) getMin).
16. Implement a stack that supports push, pop, and getMiddle in O(1).
17. Evaluate postfix expression.
18. Convert infix to postfix.
19. Sort a stack using recursion.
20. Reverse a stack using recursion.
21. Stock span problem.
22. Celebrity problem.
23. Trapping rainwater using stack.
24. Remove K digits to make the smallest number.
25. Asteroid collision.
26. Daily temperatures.

---

## 1.18 Queue

### ✅ Important Topics

- [ ] Queue operations (enqueue, dequeue, front, rear, isEmpty)
- [ ] Implementation using array and linked list
- [ ] Circular queue
- [ ] Double-ended queue (Deque)
- [ ] Priority queue
- [ ] Queue using stacks
- [ ] Sliding window maximum

### 📋 Interview Questions

1. What is a queue? What are its applications?
2. What is the difference between a queue and a deque?
3. What is a circular queue? Why is it needed?
4. How can you implement a queue using two stacks?

### 💻 Practical Coding Questions

5. Implement a queue using arrays.
6. Implement a queue using linked list.
7. Implement a queue using two stacks.
8. Implement a circular queue.
9. Sliding window maximum using deque.
10. First non-repeating character in a stream.
11. Implement a recent counter.
12. Rotting oranges (BFS).
13. Generate binary numbers from 1 to N using a queue.
14. Maximum of all subarrays of size K.
15. Interleave the first half of a queue with the second half.
16. LRU Cache using queue + hashmap.

---

## 1.19 Trees

### ✅ Important Topics

- [ ] Binary Tree
- [ ] Tree traversals (Inorder, Preorder, Postorder, Level order)
- [ ] Height/Depth of a tree
- [ ] Diameter of a tree
- [ ] Balanced binary tree
- [ ] Lowest Common Ancestor (LCA)
- [ ] Path problems
- [ ] Serialization/Deserialization
- [ ] Morris Traversal
- [ ] Tree from traversal

### 📋 Interview Questions

1. What is a binary tree? What are its types?
2. What is the difference between a full binary tree, complete binary tree, and perfect binary tree?
3. What is the maximum number of nodes at level L of a binary tree?
4. What is the maximum number of nodes in a binary tree of height H?
5. What is the difference between height and depth of a tree?
6. What is the difference between BFS and DFS for trees?

### 💻 Practical Coding Questions

7. Inorder traversal (recursive and iterative).
8. Preorder traversal (recursive and iterative).
9. Postorder traversal (recursive and iterative).
10. Level order traversal (BFS).
11. Zigzag level order traversal.
12. Find the height of a binary tree.
13. Find the diameter of a binary tree.
14. Check if a binary tree is balanced.
15. Check if two trees are identical.
16. Check if one tree is a mirror of another.
17. Find the Lowest Common Ancestor (LCA) of two nodes.
18. Find all root-to-leaf paths.
19. Maximum path sum in a binary tree.
20. Construct binary tree from inorder and preorder.
21. Construct binary tree from inorder and postorder.
22. Right side view of a binary tree.
23. Left side view of a binary tree.
24. Top view of a binary tree.
25. Bottom view of a binary tree.
26. Vertical order traversal.
27. Boundary traversal of a binary tree.
28. Flatten a binary tree to linked list.
29. Serialize and deserialize a binary tree.
30. Morris inorder traversal.
31. Count nodes in a complete binary tree.
32. Maximum width of a binary tree.
33. Check if a binary tree is symmetric.
34. Path sum problem (I, II, III).
35. Convert binary tree to its mirror.

---

## 1.20 Binary Search Tree (BST)

### ✅ Important Topics

- [ ] BST properties
- [ ] Insertion, Deletion, Search
- [ ] Inorder successor and predecessor
- [ ] Validation of BST
- [ ] Self-balancing BSTs (AVL, Red-Black Tree)
- [ ] BST to sorted list

### 📋 Interview Questions

1. What is a BST? What are its properties?
2. What is the time complexity of search, insert, and delete in a BST?
3. What happens in the worst case of a BST?
4. What is a self-balancing BST? Give examples.
5. What is the difference between AVL tree and Red-Black tree?

### 💻 Practical Coding Questions

6. Search in a BST.
7. Insert into a BST.
8. Delete a node from a BST.
9. Validate if a binary tree is a BST.
10. Find the inorder successor of a node in BST.
11. Find the inorder predecessor.
12. Find the Kth smallest element in a BST.
13. Find the Kth largest element in a BST.
14. Find the LCA of two nodes in a BST.
15. Convert a sorted array to a balanced BST.
16. Convert BST to sorted doubly linked list.
17. Merge two BSTs.
18. Find floor and ceil in a BST.
19. Two sum in a BST.
20. Recover BST (two nodes are swapped).
21. Largest BST in a binary tree.

---

## 1.21 Heap / Priority Queue

### ✅ Important Topics

- [ ] Min Heap, Max Heap
- [ ] Heap operations (insert, delete, heapify)
- [ ] Heap sort
- [ ] Priority queue
- [ ] Kth largest/smallest problems
- [ ] Median in a stream
- [ ] Merge K sorted lists

### 📋 Interview Questions

1. What is a heap? What are its types?
2. What is the time complexity of insertion and deletion in a heap?
3. What is heapify? What is its time complexity?
4. What is the difference between a heap and a BST?
5. How is a heap implemented using an array?

### 💻 Practical Coding Questions

6. Implement a min heap from scratch.
7. Kth largest element in an array.
8. Kth smallest element in an array.
9. Sort a K-sorted (nearly sorted) array.
10. Find the median from a data stream.
11. Merge K sorted lists.
12. Top K frequent elements.
13. Find K closest elements to a given value.
14. K closest points to origin.
15. Reorganize string (no two adjacent characters are the same).
16. Task scheduler.
17. Find the K most frequent words.
18. Minimum cost to connect ropes.
19. Sliding window median.
20. Ugly number II.

---

## 1.22 Trie

### ✅ Important Topics

- [ ] Trie structure
- [ ] Insert, Search, Delete
- [ ] Prefix search
- [ ] Auto-complete
- [ ] Word search
- [ ] Longest common prefix using Trie

### 📋 Interview Questions

1. What is a Trie? What are its applications?
2. What is the time complexity of insert and search in a Trie?
3. What is the space complexity of a Trie?
4. What is the difference between a Trie and a Hash Table for string storage?

### 💻 Practical Coding Questions

5. Implement a Trie (insert, search, startsWith).
6. Find the longest common prefix using a Trie.
7. Word search II (find all words in a 2D board using Trie).
8. Design an autocomplete system.
9. Count distinct substrings of a string using Trie.
10. Maximum XOR of two numbers in an array using Trie.
11. Replace words using Trie.
12. Implement a phone directory using Trie.

---

## 1.23 Graphs

### ✅ Important Topics

- [ ] Graph representation (adjacency list, adjacency matrix)
- [ ] BFS (Breadth-First Search)
- [ ] DFS (Depth-First Search)
- [ ] Cycle detection (directed and undirected graphs)
- [ ] Topological sort (Kahn's algorithm, DFS-based)
- [ ] Shortest path (Dijkstra, Bellman-Ford, Floyd-Warshall)
- [ ] Minimum spanning tree (Kruskal's, Prim's)
- [ ] Union-Find / Disjoint Set Union (DSU)
- [ ] Bipartite graph
- [ ] Strongly Connected Components (Tarjan's, Kosaraju's)
- [ ] Bridges and Articulation Points
- [ ] Graph coloring

### 📋 Interview Questions

1. What is a graph? What are its types?
2. What is the difference between BFS and DFS?
3. What is the time complexity of BFS and DFS?
4. What is the difference between adjacency list and adjacency matrix? When would you use one over the other?
5. What is a DAG (Directed Acyclic Graph)?
6. What is topological sorting? When is it used?
7. What is Dijkstra's algorithm? What are its limitations?
8. What is the difference between Dijkstra's and Bellman-Ford algorithm?
9. What is a minimum spanning tree?
10. What is the difference between Kruskal's and Prim's algorithm?
11. What is Union-Find? What is path compression and union by rank?
12. What is a bipartite graph? How do you check if a graph is bipartite?
13. What are strongly connected components?

### 💻 Practical Coding Questions

14. Implement BFS for a graph.
15. Implement DFS for a graph.
16. Find the number of connected components in an undirected graph.
17. Detect a cycle in an undirected graph (BFS and DFS).
18. Detect a cycle in a directed graph (DFS).
19. Topological sort using BFS (Kahn's algorithm).
20. Topological sort using DFS.
21. Shortest path in an unweighted graph (BFS).
22. Dijkstra's algorithm implementation.
23. Bellman-Ford algorithm implementation.
24. Floyd-Warshall algorithm implementation.
25. Kruskal's algorithm implementation.
26. Prim's algorithm implementation.
27. Check if a graph is bipartite.
28. Find the number of islands.
29. Flood fill algorithm.
30. Rotten oranges.
31. Word ladder (shortest transformation sequence).
32. Course schedule (detect cycle in directed graph).
33. Course schedule II (topological sort order).
34. Clone a graph.
35. Find all paths from source to target in a DAG.
36. Cheapest flights within K stops.
37. Network delay time.
38. Find bridges in a graph.
39. Find articulation points.
40. Kosaraju's algorithm for SCCs.
41. Alien dictionary problem.
42. Number of provinces.
43. Surrounded regions.
44. 01 Matrix (nearest 0 for each cell).
45. Pacific Atlantic water flow.
46. Accounts merge using Union-Find.

---

## 1.24 HashMap & HashSet

### ✅ Important Topics

- [ ] Hash function
- [ ] Collision handling (chaining, open addressing)
- [ ] Load factor and rehashing
- [ ] Time complexity of operations
- [ ] HashMap vs HashSet
- [ ] HashMap vs TreeMap
- [ ] Custom hash function

### 📋 Interview Questions

1. What is hashing? What is a hash function?
2. What is a collision? How do you handle collisions?
3. What is the difference between chaining and open addressing?
4. What is load factor? What happens when it exceeds a threshold?
5. What is rehashing?
6. What is the time complexity of insert, delete, and search in a hash table?
7. What is the difference between HashMap and HashSet?
8. What is the difference between HashMap and TreeMap?
9. When would you use a HashMap over a TreeMap?

### 💻 Practical Coding Questions

10. Two Sum problem.
11. Group anagrams using HashMap.
12. Find the first non-repeating character in a string.
13. Count frequency of elements in an array.
14. Check if two arrays are equal.
15. Find the longest consecutive sequence.
16. Subarray sum equals K.
17. Find all pairs with a given sum.
18. Design a HashSet from scratch.
19. Design a HashMap from scratch.
20. Longest substring without repeating characters.
21. Isomorphic strings.
22. Word pattern.
23. Find the intersection of two arrays.

---

## 1.25 Dynamic Programming (DP) Basics

### ✅ Important Topics

- [ ] Overlapping subproblems
- [ ] Optimal substructure
- [ ] Memoization (Top-down)
- [ ] Tabulation (Bottom-up)
- [ ] 1D DP
- [ ] 2D DP
- [ ] DP on strings
- [ ] DP on subsequences
- [ ] DP on grids
- [ ] Knapsack patterns (0/1, Unbounded)
- [ ] LCS, LIS
- [ ] Partition DP
- [ ] DP on stocks

### 📋 Interview Questions

1. What is dynamic programming?
2. What is the difference between memoization and tabulation?
3. What are overlapping subproblems and optimal substructure?
4. What is the difference between DP and greedy?
5. What is the difference between DP and divide and conquer?
6. How do you identify if a problem can be solved using DP?
7. What is state and transition in DP?

### 💻 Practical Coding Questions

8. Fibonacci using DP (memoization and tabulation).
9. Climbing stairs.
10. Frog jump (minimum cost).
11. House robber I and II.
12. 0/1 Knapsack problem.
13. Unbounded Knapsack.
14. Coin change (minimum coins).
15. Coin change II (number of ways).
16. Longest Common Subsequence (LCS).
17. Longest Increasing Subsequence (LIS).
18. Edit distance.
19. Longest palindromic subsequence.
20. Longest palindromic substring.
21. Minimum path sum in a grid.
22. Unique paths (I and II).
23. Subset sum problem.
24. Partition equal subset sum.
25. Target sum.
26. Rod cutting problem.
27. Matrix chain multiplication.
28. Egg dropping problem.
29. Word break problem.
30. Palindrome partitioning (minimum cuts).
31. Best time to buy and sell stock (I, II, III, IV).
32. Maximum sum increasing subsequence.
33. Count distinct subsequences.
34. Wildcard matching.
35. Regular expression matching.
36. Interleaving strings.
37. Burst balloons.
38. Minimum insertion to make a string palindrome.

---

## 1.26 Greedy Algorithms

### ✅ Important Topics

- [ ] Greedy choice property
- [ ] Greedy vs DP
- [ ] Activity selection
- [ ] Fractional knapsack
- [ ] Huffman coding
- [ ] Job sequencing
- [ ] Interval problems

### 📋 Interview Questions

1. What is a greedy algorithm?
2. What is the greedy choice property?
3. When can you use greedy over DP?
4. How do you prove a greedy algorithm is correct?

### 💻 Practical Coding Questions

5. Activity selection problem.
6. Fractional knapsack.
7. Minimum number of coins (Indian denomination).
8. Job sequencing problem.
9. Minimum platforms required at a railway station.
10. Huffman encoding.
11. N meetings in one room.
12. Assign cookies.
13. Jump game I and II.
14. Minimum number of arrows to burst balloons.
15. Non-overlapping intervals.
16. Merge intervals.
17. Candy distribution problem.
18. Lemonade change.
19. Gas station (circular tour).

---

## 1.27 Sliding Window

### ✅ Important Topics

- [ ] Fixed size sliding window
- [ ] Variable size sliding window
- [ ] Shrinking window
- [ ] Two-pointer with sliding window
- [ ] Window with HashMap/Set

### 📋 Interview Questions

1. What is the sliding window technique?
2. When do you use a fixed-size window vs variable-size window?
3. What is the difference between sliding window and two pointers?

### 💻 Practical Coding Questions

4. Maximum sum subarray of size K.
5. Longest substring without repeating characters.
6. Minimum window substring.
7. Longest substring with at most K distinct characters.
8. Fruit into baskets.
9. Maximum of all subarrays of size K.
10. Count occurrences of anagrams.
11. Longest repeating character replacement.
12. Permutation in string.
13. Subarrays with K different integers.
14. Minimum size subarray sum.

---

## 1.28 Two Pointer Technique

### ✅ Important Topics

- [ ] Two pointers from both ends
- [ ] Two pointers from same end (slow/fast)
- [ ] Three pointers
- [ ] Two pointers on sorted arrays
- [ ] Floyd's fast and slow pointer

### 📋 Interview Questions

1. What is the two-pointer technique?
2. When should you use two pointers?
3. What is the difference between two pointers and sliding window?

### 💻 Practical Coding Questions

4. Two sum in a sorted array.
5. Three sum.
6. Four sum.
7. Container with most water.
8. Remove duplicates from sorted array.
9. Move zeros to end.
10. Sort colors (Dutch National Flag).
11. Trapping rainwater.
12. Valid palindrome.
13. Merge sorted arrays.
14. Pair with given difference.
15. Find the pair closest to a target sum.

---

## 1.29 Binary Search (Advanced)

### ✅ Important Topics

- [ ] Binary search on sorted arrays
- [ ] Binary search on answer
- [ ] Binary search on rotated arrays
- [ ] Lower bound and Upper bound
- [ ] Bisect left and Bisect right
- [ ] Binary search on real numbers

### 💻 Practical Coding Questions

1. Binary search (iterative and recursive).
2. Lower bound and upper bound.
3. Find first and last position of element.
4. Count occurrences in sorted array.
5. Search in rotated sorted array (I and II).
6. Minimum in rotated sorted array.
7. Find peak element.
8. Single element in sorted array.
9. Square root of a number.
10. Kth missing positive number.
11. Find the smallest divisor given a threshold.
12. Capacity to ship packages within D days.
13. Koko eating bananas.
14. Minimum days to make M bouquets.
15. Aggressive cows / Magnetic balls.
16. Allocate minimum pages.
17. Split array largest sum.
18. Painter's partition problem.
19. Median of two sorted arrays.
20. Kth element of two sorted arrays.

---

## 1.30 Interview Coding Patterns (Must Know)

### ✅ Must Know Patterns

- [ ] Sliding Window Pattern
- [ ] Two Pointer Pattern
- [ ] Fast & Slow Pointer Pattern
- [ ] Merge Intervals Pattern
- [ ] Cyclic Sort Pattern
- [ ] In-place Reversal of LinkedList Pattern
- [ ] BFS Pattern
- [ ] DFS Pattern
- [ ] Two Heaps Pattern
- [ ] Subsets Pattern
- [ ] Modified Binary Search Pattern
- [ ] Top K Elements Pattern
- [ ] K-way Merge Pattern
- [ ] Topological Sort Pattern
- [ ] Monotonic Stack Pattern
- [ ] Prefix Sum Pattern
- [ ] Bit Manipulation Pattern
- [ ] Backtracking Pattern
- [ ] DP Patterns (Knapsack, LCS, LIS, Grid, Partition)
- [ ] Union Find Pattern
- [ ] Trie Pattern

### 📋 Pattern Recognition Questions

1. Given a problem, how do you identify which pattern to use?
2. When do you use BFS vs DFS?
3. When do you use a heap vs sorting?
4. When do you use DP vs greedy?
5. When do you use a Trie vs HashMap for string problems?
6. When do you use Union-Find vs DFS for connectivity problems?
7. How do you identify a sliding window problem?
8. How do you identify a two-pointer problem?
9. How do you identify a binary search on answer problem?
10. How do you identify a monotonic stack problem?

### 🎯 What Interviewer Expects

- [ ] Clean, readable code with proper variable names
- [ ] Explain approach before coding
- [ ] Discuss time and space complexity
- [ ] Consider edge cases
- [ ] Optimize from brute force to optimal
- [ ] Test with examples
- [ ] Handle follow-up questions gracefully

### ❌ Common Mistakes

- [ ] Jumping straight to code without understanding the problem
- [ ] Not considering edge cases (empty array, single element, negative numbers)
- [ ] Not analyzing time and space complexity
- [ ] Writing unreadable code with single-letter variables
- [ ] Not testing the solution with examples
- [ ] Giving up too quickly on hard problems
- [ ] Not communicating thought process
- [ ] Ignoring integer overflow
- [ ] Off-by-one errors in binary search
- [ ] Not handling null/undefined inputs
- [ ] Assuming sorted input when it's not stated
- [ ] Modifying input array when not allowed

---

> **📌 SECTION 1 COMPLETE — Programming Fundamentals**

---

# ═══════════════════════════════════════════════════════