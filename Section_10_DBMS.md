# ═══════════════════════════════════════════════════════
# SECTION 10: DBMS (DATABASE MANAGEMENT SYSTEMS)
# ═══════════════════════════════════════════════════════

---

## 10.1 DBMS Basics & Architecture

### ✅ Important Topics
- [ ] What is a DBMS?
- [ ] File System vs DBMS
- [ ] 3-Tier Architecture (Physical, Logical, View level)
- [ ] Data Independence
- [ ] ER Diagrams (Entities, Attributes, Relationships)
- [ ] Types of Keys (Primary, Foreign, Candidate, Super, Alternate, Composite)

### 📋 Interview Questions
1. What is a Database Management System (DBMS)? What are its advantages over a traditional file system?
2. Explain the 3-schema architecture of a DBMS (Internal, Conceptual, External levels).
3. What is Data Independence? Explain logical and physical data independence.
4. What is an Entity-Relationship (ER) Diagram? What are its main components?
5. What is the difference between a weak entity and a strong entity?
6. Define Primary Key, Foreign Key, and Candidate Key.
7. What is the difference between a Super Key and a Candidate Key?
8. What is a Composite Key?

---

## 10.2 Normalization

### ✅ Important Topics
- [ ] Purpose of Normalization (Data Redundancy, Anomalies)
- [ ] Insertion, Updation, and Deletion Anomalies
- [ ] Functional Dependency
- [ ] 1NF, 2NF, 3NF, BCNF
- [ ] Denormalization

### 📋 Interview Questions
1. What is Normalization? Why do we need it?
2. What are Data Anomalies? Give examples of Insertion, Updation, and Deletion anomalies.
3. What is Functional Dependency in a database?
4. Explain First Normal Form (1NF).
5. Explain Second Normal Form (2NF). What is a partial dependency?
6. Explain Third Normal Form (3NF). What is a transitive dependency?
7. What is BCNF (Boyce-Codd Normal Form)? How is it different from 3NF?
8. What is Denormalization? Why would you intentionally denormalize a database?

---

## 10.3 Relational Algebra & Joins

### ✅ Important Topics
- [ ] Relational Algebra vs Relational Calculus
- [ ] Inner Join, Left Join, Right Join, Full Outer Join
- [ ] Cross Join, Self Join
- [ ] Natural Join vs Equi Join

### 📋 Interview Questions
1. What is Relational Algebra? Name the fundamental operations.
2. What is a JOIN in DBMS?
3. Explain the difference between an INNER JOIN and a LEFT OUTER JOIN.
4. What is a FULL OUTER JOIN?
5. What is a CROSS JOIN (Cartesian Product)? When does a CROSS JOIN act like an INNER JOIN?
6. What is a SELF JOIN? Give a practical example of when you would use it.
7. What is a NATURAL JOIN? How does it differ from a standard INNER JOIN?

---

## 10.4 Transactions & Concurrency Control

### ✅ Important Topics
- [ ] What is a Transaction?
- [ ] ACID Properties
- [ ] Concurrency Problems (Dirty Read, Non-repeatable Read, Phantom Read)
- [ ] Isolation Levels (Read Uncommitted, Read Committed, Repeatable Read, Serializable)
- [ ] Locking Protocols (Shared Lock, Exclusive Lock, 2PL)
- [ ] Deadlock in DBMS

### 📋 Interview Questions
1. What is a Database Transaction?
2. Explain the ACID properties of a transaction in detail.
3. What is Concurrency Control? Why is it needed in a DBMS?
4. What is a Dirty Read? Which isolation level allows it?
5. What is a Non-repeatable Read? How is it different from a Phantom Read?
6. Explain the four Isolation Levels defined by the SQL standard. Which one is the strictest?
7. What is the difference between a Shared Lock (S-Lock) and an Exclusive Lock (X-Lock)?
8. What is the Two-Phase Locking (2PL) protocol? How does it guarantee serializability?
9. What is a Deadlock in a DBMS? How can it be prevented or resolved?

---

## 10.5 Indexes & Distributed Databases

### ✅ Important Topics
- [ ] Indexing basics
- [ ] Clustered vs Non-Clustered Indexes
- [ ] B-Trees and B+ Trees
- [ ] CAP Theorem (Consistency, Availability, Partition Tolerance)

### 📋 Interview Questions
1. What is an Index in a database? How does it improve read performance?
2. What is the tradeoff of adding an index? (Slower writes/updates, storage overhead).
3. Explain the difference between a Clustered Index and a Non-Clustered Index.
4. How many Clustered Indexes can a single table have? Why?
5. Why are B-Trees and B+ Trees used for database indexing instead of Binary Search Trees?
6. What is the CAP Theorem in distributed databases?
7. According to the CAP Theorem, why can't a distributed database guarantee all three properties simultaneously during a network partition?

---

### 🎯 What Interviewer Expects (DBMS)
- [ ] Crystal clear understanding of Normalization up to BCNF.
- [ ] Flawless explanation of ACID properties.
- [ ] Deep understanding of Concurrency problems (Dirty/Phantom reads) and how Isolation levels solve them.
- [ ] Ability to design a basic ER diagram for a real-world scenario (e.g., E-commerce, Library).

### ❌ Common Mistakes (DBMS)
- [ ] Memorizing Normalization definitions without understanding functional dependencies.
- [ ] Confusing Primary Key, Candidate Key, and Super Key.
- [ ] Thinking Denormalization is always bad (it is heavily used in read-heavy systems and data warehouses).

---

> **📌 SECTION 10 COMPLETE — DBMS**
>
> Say **"Continue"** to generate **Section 11: Git & GitHub**

---
