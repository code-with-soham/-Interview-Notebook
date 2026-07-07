# ═══════════════════════════════════════════════════════
# SECTION 13: C++ & PYTHON (LANGUAGE SPECIFICS)
# ═══════════════════════════════════════════════════════

---

## 13.1 C++ Fundamentals & Memory Management

### ✅ Important Topics
- [ ] Pointers vs References
- [ ] Memory Allocation (new, delete, malloc, free)
- [ ] Memory Leaks & Dangling Pointers
- [ ] Smart Pointers (unique_ptr, shared_ptr, weak_ptr)
- [ ] Object-Oriented Programming in C++ (Virtual Functions, Abstract Classes, vtable)
- [ ] RAII (Resource Acquisition Is Initialization)
- [ ] STL (Standard Template Library) - Vectors, Maps, Sets
- [ ] Pass by Value vs Pass by Reference vs Pass by Pointer

### 📋 Interview Questions
1. What is the difference between a pointer and a reference in C++?
2. Explain `new` and `delete` vs `malloc` and `free`.
3. What is a Memory Leak? How do you prevent it in C++?
4. What is a Dangling Pointer? What is a Wild Pointer?
5. What are Smart Pointers in C++11? Explain `std::unique_ptr` and `std::shared_ptr`.
6. What is a Virtual Function? What is a Pure Virtual Function?
7. Explain the concept of a vtable (Virtual Table) and vptr (Virtual Pointer).
8. What is RAII? Why is it considered a core idiom in C++?
9. What happens if a destructor throws an exception?
10. Differentiate between `std::vector` and `std::list`. When would you use which?
11. How does `std::map` work internally? (Red-Black Tree). How is it different from `std::unordered_map`? (Hash Table).
12. What is the `const` keyword used for? Explain `const` pointers vs pointers to `const`.

### 💻 Code Snippet Questions
13. What is wrong with this code?
```cpp
int* ptr = new int(10);
delete ptr;
*ptr = 20; // What happens here?
```

14. How do you implement a Singleton class in C++?

---

## 13.2 Python Fundamentals

### ✅ Important Topics
- [ ] Interpreted vs Compiled Languages
- [ ] Dynamic Typing vs Static Typing
- [ ] Mutable vs Immutable Data Types
- [ ] Lists, Tuples, Sets, Dictionaries
- [ ] List Comprehensions
- [ ] Generators and `yield`
- [ ] Decorators
- [ ] Global Interpreter Lock (GIL)
- [ ] Memory Management & Garbage Collection
- [ ] `__init__`, `__str__`, `__repr__` (Dunder methods)

### 📋 Interview Questions
1. Is Python interpreted or compiled? (Answer: Both, compiled to bytecode, then interpreted by PVM).
2. What is the difference between dynamically typed and statically typed languages?
3. Which data types in Python are mutable, and which are immutable? (List/Dict/Set vs String/Tuple/Int).
4. What is the difference between a List and a Tuple?
5. How does a Dictionary work internally in Python?
6. What is a List Comprehension? Give an example.
7. What is a Generator? How is it different from a regular function returning a list?
8. What does the `yield` keyword do?
9. What is a Decorator in Python? How would you write a simple timing decorator?
10. What is the Global Interpreter Lock (GIL) in CPython? How does it affect multithreading?
11. How does Python manage memory? (Reference counting and Garbage Collection).
12. What is the difference between `==` and `is` in Python?
13. What is the difference between deep copy and shallow copy?
14. What are `*args` and `**kwargs`?
15. What are lambda functions?

### 💻 Code Snippet Questions
16. What is the output of this code?
```python
def append_to_list(val, my_list=[]):
    my_list.append(val)
    return my_list

print(append_to_list(1))
print(append_to_list(2))
# Why doesn't the second print output [2]?
```

17. Write a list comprehension to square all even numbers from 1 to 10.

---

## 13.3 C++ vs Python vs JavaScript (Comparison)

### 📋 Interview Questions
1. Compare memory management in C++, Python, and JavaScript.
2. If you need to build a high-frequency trading application, which language would you choose and why?
3. If you need to build a rapid prototype for a web application, which language would you choose and why?
4. How is multi-threading different in C++, Python, and Node.js?
5. Compare the execution speed of C++ vs Python. Why is Python slower?

---

### 🎯 What Interviewer Expects
- [ ] **C++:** Deep understanding of memory management, pointers, and object-oriented principles.
- [ ] **Python:** Understanding of Python's quirks (mutability default arguments), GIL, generators, and decorators.
- [ ] **General:** The ability to choose the right language for the right task (C++ for performance, Python for scripts/AI/data, JS for web).

### ❌ Common Mistakes
- [ ] **C++:** Confusing references with pointers. Not knowing how `virtual` functions work.
- [ ] **Python:** Modifying a list while iterating over it. Not understanding why default mutable arguments (like `def func(lst=[])`) are dangerous.

---

> **📌 SECTION 13 COMPLETE — C++ & Python**
