# ═══════════════════════════════════════════════════════
# SECTION 22: TOP 100 MOST REPEATED INTERVIEW QUESTIONS
# ═══════════════════════════════════════════════════════

*Context: Based on thousands of interview experiences, these 100 questions are statistically the most likely to be asked depending on the type of company you are interviewing with.*

---

## 🏢 FAANG & Product Giants (Google, Amazon, Microsoft, Adobe, Oracle)
*Focus: Heavy Data Structures & Algorithms, System Design, and Low-Level Architecture.*

### DSA & Problem Solving
1. Given an array of integers, find two numbers such that they add up to a specific target (Two Sum).
2. Find the longest substring without repeating characters.
3. Merge overlapping intervals in a 2D array.
4. Search for a target value in a rotated sorted array.
5. Given a linked list, detect if it has a cycle and find the starting node of the cycle.
6. Reverse a linked list in groups of size k.
7. Implement an LRU (Least Recently Used) Cache.
8. Find the lowest common ancestor of two nodes in a Binary Tree.
9. Serialize and Deserialize a Binary Tree.
10. Find the maximum path sum in a Binary Tree.
11. Number of Islands (Count connected components in a 2D grid).
12. Clone a graph.
13. Implement a Trie (Prefix Tree).
14. Word Break (Dynamic Programming).
15. Trapping Rain Water.

### Core CS & System Design (Entry Level)
16. How does a HashMap work internally in memory? What happens during a collision?
17. Explain the difference between a Mutex and a Semaphore with a real-world example.
18. What happens when you type `google.com` into your browser? (Deep dive into DNS, TCP, TLS).
19. Explain the ACID properties of a database transaction.
20. What is the difference between TCP and UDP? When would you use UDP?
21. What is a Deadlock? How do you prevent it?
22. Explain Virtual Memory and Paging.
23. How would you design a URL Shortener (like bit.ly)?
24. How would you design a Rate Limiter?
25. Explain the CAP Theorem.

### Behavioral (Leadership Principles)
26. Tell me about a time you had to dive deep into a problem to figure out the root cause.
27. Describe a time you disagreed with a manager or peer. How did you resolve it?
28. Tell me about a time you had to deliver a project under a very tight deadline.
29. Describe a situation where you had to learn something completely new to solve a problem.
30. Tell me about a time you made a mistake that affected a customer.

---

## 🏢 Indian Product Giants (Flipkart, Swiggy, Zomato, PhonePe, Meesho)
*Focus: Scale, Database Optimization, Concurrency, and Practical Problem Solving.*

### Technical & Architecture
31. How do you implement pagination for an API returning 10 million records?
32. What is the difference between clustered and non-clustered indexes?
33. Explain how you would optimize a slow-running SQL query.
34. What is caching? Where would you put a Redis cache in your architecture?
35. How does the Event Loop work in Node.js? How does it handle thousands of concurrent requests?
36. What is the difference between `Promise.all` and `Promise.allSettled`?
37. How do you handle race conditions in an asynchronous environment?
38. Explain the difference between WebSockets and Server-Sent Events (SSE).
39. How do you handle authentication in a microservices architecture?
40. Explain how JWT works. What are the security risks of storing it in `localStorage`?
41. How would you design the "Add to Cart" functionality for high concurrency (Flash Sale)?
42. How would you design a Delivery Tracking system (like Swiggy)?
43. What is Database Sharding? How does it differ from Replication?
44. Explain the difference between normalization and denormalization.
45. How do you handle API Rate Limiting?

### Coding & Output Based
46. Sort an array of 0s, 1s, and 2s without using extra space (Dutch National Flag).
47. Find the next greater element for every element in an array.
48. Flatten a deeply nested JavaScript object or array.
49. Write a polyfill for `Array.prototype.map()` or `Function.prototype.bind()`.
50. What is the output of `setTimeout(..., 0)` inside a Promise `.then()`?

---

## 🏢 Service-Based Giants (TCS, Infosys, Wipro, Cognizant, Accenture)
*Focus: Core Computer Science Fundamentals, OOP Concepts, Basic DSA, and SQL.*

### OOP & Core Concepts
51. What are the four pillars of Object-Oriented Programming (OOP)?
52. What is the difference between Overloading and Overriding?
53. What is a Virtual Function in C++?
54. Can we instantiate an abstract class? Why or why not?
55. What is the difference between a pointer and a reference?
56. Explain the difference between `malloc/free` and `new/delete`.
57. What is a Memory Leak? How do you avoid it?
58. What is the difference between a Primary Key and a Unique Key?
59. What is a Foreign Key?
60. What is a Left Outer Join? Write a SQL query demonstrating it.
61. What is a View in SQL?
62. What is normalization? Explain 1NF, 2NF, and 3NF.
63. Explain the different states of a Process in an Operating System.
64. What is a Zombie Process?
65. What is the difference between an Array and a Linked List?

### Basic Coding & Logic
66. Write a program to reverse a string without using built-in functions.
67. Write a program to check if a string is a palindrome.
68. Write a program to find the factorial of a number using recursion.
69. Write a program to check if a number is Prime.
70. Write a program to print the Fibonacci series up to N terms.
71. Write a program to find the second largest element in an array.
72. Write a program to swap two numbers without using a third variable.
73. Write a program to detect if two strings are anagrams of each other.
74. Write a program to count the frequency of characters in a string.
75. Explain the concept of Binary Search. What is its time complexity?

---

## 🏢 Modern Startups & AI Companies
*Focus: MERN Stack mastery, React Internals, API Integration, AI/LLMs, and "Building things quickly".*

### MERN & Frontend
76. Explain the React component lifecycle (or the equivalent `useEffect` hooks).
77. What is the Virtual DOM? Why does it make React fast?
78. What is the difference between `useMemo` and `useCallback`?
79. How do you prevent unnecessary re-renders in a React application?
80. What is Prop Drilling, and how do you solve it using Zustand or Context API?
81. How does Redux differ from Zustand?
82. Explain Server-Side Rendering (SSR) vs Client-Side Rendering (CSR).
83. What is CSS Specificity?
84. How do you center a div horizontally and vertically using Flexbox?
85. Explain how CORS (Cross-Origin Resource Sharing) works and how to bypass/fix CORS errors.

### Backend, APIs & Deployment
86. Walk me through how you implemented Authentication (OTP/JWT) in CampusHub.
87. How do you securely hash and store passwords in a database?
88. What is middleware in Express.js? Give an example of a custom middleware you wrote.
89. How do you deploy a React frontend and a Node backend using Docker?
90. Explain how a CI/CD pipeline works (e.g., GitHub Actions).

### AI, RAG & LLMs
91. What is Prompt Engineering? Provide an example of a good vs bad prompt.
92. How does the Groq API achieve lower latency compared to OpenAI?
93. What is a Vector Database? How is it different from MongoDB?
94. Explain the full Retrieval-Augmented Generation (RAG) architecture.
95. What are Embeddings? How do they capture semantic meaning?
96. How do you handle the token context window limit when building an AI chat application?
97. What is Prompt Injection, and how do you secure an LLM against it?
98. What is Temperature in an LLM? When would you use a temperature of 0?
99. Explain Function Calling (Tool Use) in the context of AI Agents.
100. How do you prevent an AI from hallucinating incorrect facts?

---

> **📌 SECTION 22 COMPLETE — Top 100 Most Repeated Questions**
>
> Say **"Continue"** to generate the final section: **Section 23: Mistakes Freshers Make**

---
