# ═══════════════════════════════════════════════════════
# SECTION 6: SQL & MySQL (COMPLETE)
# ═══════════════════════════════════════════════════════

---

## 6.1 SQL Fundamentals

### ✅ Important Topics
- [ ] What is SQL
- [ ] SQL vs NoSQL
- [ ] DDL (CREATE, ALTER, DROP, TRUNCATE, RENAME)
- [ ] DML (INSERT, UPDATE, DELETE, SELECT)
- [ ] DCL (GRANT, REVOKE)
- [ ] TCL (COMMIT, ROLLBACK, SAVEPOINT)
- [ ] Data types (INT, VARCHAR, TEXT, DATE, DATETIME, FLOAT, BOOLEAN, ENUM, BLOB)
- [ ] NULL handling
- [ ] Aliases
- [ ] Comments in SQL
- [ ] SQL execution order

### 📋 Interview Questions
1. What is SQL? What does it stand for?
2. What is the difference between SQL and NoSQL?
3. What is the difference between DDL, DML, DCL, and TCL?
4. What is the difference between `DELETE`, `TRUNCATE`, and `DROP`?
5. What is the difference between `CHAR` and `VARCHAR`?
6. What is `NULL` in SQL? Is NULL equal to 0 or empty string?
7. What is the order of SQL query execution? (FROM → WHERE → GROUP BY → HAVING → SELECT → ORDER BY → LIMIT)
8. What is an alias in SQL?
9. What is the difference between `WHERE` and `HAVING`?
10. What is the difference between `DELETE` and `TRUNCATE`?
11. What is the difference between `DROP` and `TRUNCATE`?
12. Can you rollback after `TRUNCATE`? After `DELETE`?

---

## 6.2 SELECT Queries

### ✅ Important Topics
- [ ] SELECT, FROM, WHERE
- [ ] DISTINCT
- [ ] ORDER BY (ASC, DESC)
- [ ] LIMIT, OFFSET
- [ ] WHERE operators (=, !=, <, >, <=, >=, BETWEEN, IN, NOT IN, LIKE, IS NULL, IS NOT NULL)
- [ ] Wildcard characters (%, _)
- [ ] AND, OR, NOT
- [ ] Aggregate functions (COUNT, SUM, AVG, MIN, MAX)
- [ ] GROUP BY
- [ ] HAVING
- [ ] CASE WHEN

### 📋 Interview Questions
1. How do you select all columns from a table?
2. How do you select distinct values?
3. How do you sort results in ascending/descending order?
4. What is the `LIKE` operator? What are `%` and `_` wildcards?
5. What is the difference between `BETWEEN` and using `>=` and `<=`?
6. What is the `IN` operator?
7. How do you filter NULL values?
8. What are aggregate functions? Name them.
9. What is `GROUP BY`? When do you use it?
10. What is `HAVING`? How is it different from `WHERE`?
11. What is `CASE WHEN`? Give an example.
12. How do you implement pagination in SQL?

### 💻 Practical SQL Questions
13. Find all employees with salary greater than 50000.
14. Find the top 5 highest-paid employees.
15. Find the total salary expense per department.
16. Find departments with more than 10 employees.
17. Find the second highest salary in the employees table.
18. Find the Nth highest salary.
19. Find employees whose name starts with 'A' and ends with 'n'.
20. Find the average salary per department, sorted by average salary descending.
21. Count the number of employees in each city.
22. Find employees who joined in the last 30 days.
23. Write a query to classify employees as 'Junior' (< 2 years), 'Mid' (2-5 years), 'Senior' (> 5 years).

---

## 6.3 Joins

### ✅ Important Topics
- [ ] INNER JOIN
- [ ] LEFT JOIN (LEFT OUTER JOIN)
- [ ] RIGHT JOIN (RIGHT OUTER JOIN)
- [ ] FULL OUTER JOIN
- [ ] CROSS JOIN
- [ ] SELF JOIN
- [ ] NATURAL JOIN
- [ ] Join conditions (ON, USING)
- [ ] Multiple table joins
- [ ] Anti-join patterns

### 📋 Interview Questions
1. What is a JOIN in SQL? Why is it needed?
2. What is the difference between INNER JOIN and LEFT JOIN?
3. What is a RIGHT JOIN?
4. What is a FULL OUTER JOIN?
5. What is a CROSS JOIN? What is a Cartesian product?
6. What is a SELF JOIN? Give a real-world example.
7. What is a NATURAL JOIN?
8. What is the difference between ON and USING in joins?
9. Can you join more than two tables?
10. What is an anti-join? How do you find records that don't match?
11. How do you find employees who don't belong to any department?
12. What is the performance impact of joins on large tables?

### 💻 Practical SQL Questions
13. List all employees with their department names (INNER JOIN).
14. List all departments, including those with no employees (LEFT JOIN).
15. Find employees who are managers of other employees (SELF JOIN).
16. Find customers who have never placed an order.
17. Find common products between two tables.
18. Join three tables: employees, departments, and locations.
19. Find the department with the most employees using JOIN + GROUP BY.
20. Find all pairs of employees from the same department.

---

## 6.4 Subqueries

### ✅ Important Topics
- [ ] Scalar subquery
- [ ] Row subquery
- [ ] Table subquery
- [ ] Correlated subquery
- [ ] Non-correlated subquery
- [ ] EXISTS / NOT EXISTS
- [ ] IN with subquery
- [ ] ANY, ALL
- [ ] Subquery in SELECT, FROM, WHERE

### 📋 Interview Questions
1. What is a subquery?
2. What is the difference between a correlated and non-correlated subquery?
3. What is a scalar subquery?
4. Where can you use subqueries? (SELECT, FROM, WHERE, HAVING)
5. What is the `EXISTS` keyword?
6. What is the difference between `IN` and `EXISTS`?
7. What is the difference between `ANY` and `ALL`?
8. When should you use a subquery vs a JOIN?
9. Can subqueries return multiple columns?
10. What is a derived table?

### 💻 Practical SQL Questions
11. Find employees whose salary is above the average salary.
12. Find the department with the highest average salary.
13. Find employees who earn more than their department average.
14. Find the second highest salary using a subquery.
15. Find customers who placed orders in the last month (using EXISTS).
16. Find products that have never been ordered.
17. Find employees who work in the same department as 'John'.
18. Find departments where all employees earn more than 30000.

---

## 6.5 Views

### ✅ Important Topics
- [ ] What is a view
- [ ] CREATE VIEW
- [ ] Updatable views
- [ ] Materialized views
- [ ] View advantages and disadvantages
- [ ] View vs Table

### 📋 Interview Questions
1. What is a view in SQL?
2. How do you create a view?
3. Can you update data through a view?
4. What is a materialized view? How is it different from a regular view?
5. What are the advantages of using views?
6. What are the limitations of views?
7. Can you create an index on a view?
8. What is the difference between a view and a table?
9. When would you use a view?
10. How do you drop a view?

---

## 6.6 Triggers & Stored Procedures

### ✅ Important Topics
- [ ] Triggers (BEFORE, AFTER, INSTEAD OF)
- [ ] Trigger events (INSERT, UPDATE, DELETE)
- [ ] Stored Procedures
- [ ] Functions (User-Defined Functions)
- [ ] Cursors
- [ ] Difference between procedures and functions
- [ ] Parameters (IN, OUT, INOUT)

### 📋 Interview Questions
1. What is a trigger in SQL?
2. What are the types of triggers? (BEFORE, AFTER)
3. On what events can triggers fire?
4. What is a stored procedure?
5. What is the difference between a stored procedure and a function?
6. What are the advantages of stored procedures?
7. What is a cursor? When would you use one?
8. What is the difference between IN, OUT, and INOUT parameters?
9. Can a trigger call a stored procedure?
10. What are the disadvantages of triggers?
11. How do you create a trigger that logs changes to an audit table?
12. Can you have multiple triggers on the same table?

---

## 6.7 Constraints

### ✅ Important Topics
- [ ] PRIMARY KEY
- [ ] FOREIGN KEY
- [ ] UNIQUE
- [ ] NOT NULL
- [ ] CHECK
- [ ] DEFAULT
- [ ] AUTO_INCREMENT / SERIAL
- [ ] Composite keys
- [ ] Referential integrity
- [ ] CASCADE, SET NULL, RESTRICT, NO ACTION

### 📋 Interview Questions
1. What are constraints in SQL?
2. What is a PRIMARY KEY? Can it be NULL?
3. What is a FOREIGN KEY? Why is it important?
4. What is the difference between PRIMARY KEY and UNIQUE?
5. Can a table have multiple PRIMARY KEYs?
6. Can a table have multiple UNIQUE constraints?
7. What is the CHECK constraint?
8. What is the DEFAULT constraint?
9. What is a composite key?
10. What is referential integrity?
11. What is CASCADE DELETE? When would you use it?
12. What is the difference between CASCADE, SET NULL, and RESTRICT?
13. What is AUTO_INCREMENT?
14. Can a FOREIGN KEY reference a non-PRIMARY KEY column?

---

## 6.8 Indexes in SQL

### ✅ Important Topics
- [ ] Clustered index
- [ ] Non-clustered index
- [ ] Unique index
- [ ] Composite index
- [ ] Covering index
- [ ] Full-text index
- [ ] B-Tree index
- [ ] Hash index
- [ ] Index optimization
- [ ] EXPLAIN / EXPLAIN ANALYZE

### 📋 Interview Questions
1. What is an index in SQL?
2. What is the difference between a clustered and non-clustered index?
3. How many clustered indexes can a table have?
4. What is a composite index?
5. What is a covering index?
6. What is a B-Tree? How do database indexes use it?
7. When should you create an index?
8. When should you NOT create an index?
9. What is the impact of indexes on INSERT, UPDATE, DELETE?
10. How do you analyze a query's execution plan?
11. What is `EXPLAIN` in MySQL?
12. What is index selectivity?
13. Can you have an index on a NULL column?
14. What is a full-text index?

### 🎯 Scenario Based Questions
15. A SELECT query on a 50-million row table is slow. How do you optimize?
16. You have a query that filters on columns A, B, and C. What index would you create?
17. After adding an index, INSERT operations became slow. Why?

---

## 6.9 Normalization

### ✅ Important Topics
- [ ] Database normalization concept
- [ ] 1NF (First Normal Form)
- [ ] 2NF (Second Normal Form)
- [ ] 3NF (Third Normal Form)
- [ ] BCNF (Boyce-Codd Normal Form)
- [ ] Denormalization
- [ ] Functional dependency
- [ ] Candidate key, Super key, Primary key

### 📋 Interview Questions
1. What is normalization? Why is it important?
2. What are the different normal forms?
3. What is 1NF? Give an example of a table that violates 1NF.
4. What is 2NF? What is partial dependency?
5. What is 3NF? What is transitive dependency?
6. What is BCNF?
7. What is denormalization? When would you denormalize?
8. What is a functional dependency?
9. What is the difference between a candidate key and a super key?
10. What are the advantages and disadvantages of normalization?
11. How is normalization different from denormalization?
12. Normalize a given table step by step (1NF → 2NF → 3NF).

### 💻 Practical Questions
13. Given a table: `StudentCourse(student_id, student_name, course_id, course_name, instructor)`. Normalize it to 3NF.
14. Given a denormalized order table, normalize it to 3NF.
15. When would you choose denormalization over normalization?

---

## 6.10 Transactions & ACID

### ✅ Important Topics
- [ ] Transaction concept
- [ ] ACID properties (Atomicity, Consistency, Isolation, Durability)
- [ ] COMMIT
- [ ] ROLLBACK
- [ ] SAVEPOINT
- [ ] Isolation levels (Read Uncommitted, Read Committed, Repeatable Read, Serializable)
- [ ] Concurrency problems (Dirty Read, Non-Repeatable Read, Phantom Read)
- [ ] Locking (Shared, Exclusive)
- [ ] Deadlock

### 📋 Interview Questions
1. What is a transaction in SQL?
2. What are ACID properties? Explain each.
3. What is Atomicity?
4. What is Consistency?
5. What is Isolation?
6. What is Durability?
7. What is COMMIT? What is ROLLBACK?
8. What is a SAVEPOINT?
9. What are isolation levels? Name all four.
10. What is a dirty read?
11. What is a non-repeatable read?
12. What is a phantom read?
13. Which isolation level prevents all concurrency problems?
14. What is the default isolation level in MySQL?
15. What is a deadlock? How do you prevent it?
16. What is the difference between shared and exclusive locks?
17. What is optimistic locking vs pessimistic locking?

### 🎯 Scenario Based Questions
18. Two users try to update the same row at the same time. What happens?
19. A bank transfer needs to debit one account and credit another. How do you ensure consistency?
20. Your application has many read operations and few writes. What isolation level would you choose?

---

## 6.11 Advanced SQL Queries

### ✅ Important Topics
- [ ] Window functions (ROW_NUMBER, RANK, DENSE_RANK, NTILE)
- [ ] OVER clause (PARTITION BY, ORDER BY)
- [ ] LEAD, LAG
- [ ] FIRST_VALUE, LAST_VALUE
- [ ] Common Table Expressions (CTE)
- [ ] Recursive CTE
- [ ] UNION, UNION ALL, INTERSECT, EXCEPT
- [ ] String functions (CONCAT, SUBSTRING, UPPER, LOWER, TRIM, REPLACE, LENGTH)
- [ ] Date functions (NOW, CURDATE, DATEDIFF, DATE_ADD, DATE_FORMAT)
- [ ] COALESCE, IFNULL, NULLIF
- [ ] CAST and CONVERT

### 📋 Interview Questions
1. What are window functions? How are they different from aggregate functions?
2. What is `ROW_NUMBER()`?
3. What is the difference between `RANK()`, `DENSE_RANK()`, and `ROW_NUMBER()`?
4. What is the `OVER` clause?
5. What is `PARTITION BY`?
6. What are `LEAD()` and `LAG()`?
7. What is a CTE? How is it different from a subquery?
8. What is a recursive CTE? Give an example.
9. What is the difference between `UNION` and `UNION ALL`?
10. What is `COALESCE()`?
11. What is `IFNULL()`?
12. What is `NULLIF()`?

### 💻 Practical SQL Questions
13. Find the rank of each employee by salary within their department.
14. Find the running total of sales by month.
15. Find the difference in salary between an employee and the previous employee (using LAG).
16. Find the top 3 earners in each department using `ROW_NUMBER()`.
17. Write a recursive CTE to find all employees in an organizational hierarchy.
18. Find duplicate records in a table.
19. Delete duplicate records keeping only the first occurrence.
20. Find the cumulative sum of a column.
21. Find employees whose salary is above the average of their department (using window functions).
22. Find the median salary.
23. Swap values of two columns in a table.
24. Find the consecutive days a user logged in.
25. Pivot rows into columns.

---

## 6.12 SQL Optimization

### ✅ Important Topics
- [ ] Query optimization techniques
- [ ] EXPLAIN / EXPLAIN ANALYZE
- [ ] Index optimization
- [ ] Avoiding SELECT *
- [ ] Avoiding unnecessary subqueries
- [ ] Using LIMIT
- [ ] Batch operations
- [ ] Query caching
- [ ] Connection pooling
- [ ] Partitioning

### 📋 Interview Questions
1. How do you optimize SQL queries?
2. Why is SELECT * bad?
3. How do you use EXPLAIN to analyze a query?
4. What is a full table scan? How do you avoid it?
5. How does indexing improve query performance?
6. What is query caching?
7. What is table partitioning? When would you use it?
8. What are the common causes of slow SQL queries?
9. How do you optimize JOIN queries?
10. What is the difference between a correlated subquery and a join in terms of performance?

### 🎯 Scenario Based Questions
11. You have a query that takes 30 seconds. How do you troubleshoot?
12. A report query joins 5 tables with millions of rows. How do you optimize it?
13. Your database is running out of storage. What strategies can you use?
14. You need to insert 1 million rows efficiently. How do you do it?

---

### 🎯 What Interviewer Expects (SQL)
- [ ] Ability to write complex queries with joins, subqueries, and aggregations
- [ ] Understanding of normalization and when to denormalize
- [ ] Knowledge of indexes and query optimization
- [ ] Understanding of ACID properties and isolation levels
- [ ] Ability to solve scenario-based SQL problems
- [ ] Knowledge of window functions (ROW_NUMBER, RANK, LEAD, LAG)
- [ ] Understanding of transactions and locking
- [ ] Ability to design database schemas

### ❌ Common Mistakes (SQL)
- [ ] Using SELECT * in production queries
- [ ] Not using indexes on frequently queried columns
- [ ] Confusing WHERE and HAVING
- [ ] Not understanding NULL behavior in comparisons
- [ ] Using correlated subqueries when a JOIN would be faster
- [ ] Not considering the order of SQL clause execution
- [ ] Over-normalizing or under-normalizing
- [ ] Not using transactions for multi-step operations
- [ ] Not understanding the difference between DELETE and TRUNCATE
- [ ] Confusing UNION and UNION ALL

---

> **📌 SECTION 6 COMPLETE — SQL & MySQL**
>
> Say **"Continue"** to generate **Section 7: System Design** + **Section 8: Operating System**

---
