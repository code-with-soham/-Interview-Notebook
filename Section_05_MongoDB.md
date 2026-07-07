# ═══════════════════════════════════════════════════════
# SECTION 5: MONGODB (COMPLETE)
# ═══════════════════════════════════════════════════════

---

## 5.1 MongoDB Fundamentals

### ✅ Important Topics
- [ ] What is MongoDB (NoSQL, document-oriented)
- [ ] MongoDB vs SQL databases
- [ ] Documents, Collections, Databases
- [ ] BSON format
- [ ] _id field and ObjectId
- [ ] MongoDB data types
- [ ] mongo shell / mongosh
- [ ] MongoDB Compass
- [ ] MongoDB Atlas (cloud)
- [ ] Mongoose ODM
- [ ] Connection string and connection pooling
- [ ] When to use MongoDB vs SQL

### 📋 Interview Questions
1. What is MongoDB? What type of database is it?
2. What is the difference between SQL and NoSQL databases?
3. What is a document in MongoDB?
4. What is a collection in MongoDB?
5. What is BSON? How is it different from JSON?
6. What is `_id` in MongoDB? Can you customize it?
7. What is an ObjectId? What information does it contain?
8. What are the data types supported by MongoDB?
9. What is Mongoose? Why do we use it?
10. What is the difference between Mongoose and the native MongoDB driver?
11. What is MongoDB Atlas?
12. When should you use MongoDB over a SQL database?
13. When should you NOT use MongoDB?
14. What is a connection string in MongoDB?
15. What is connection pooling? Why is it important?
16. What is the maximum document size in MongoDB?
17. What is the difference between MongoDB and CouchDB?
18. What are the advantages and disadvantages of MongoDB?

### 🎯 Scenario Based Questions
19. You're building a social media app. Would you choose MongoDB or PostgreSQL? Why?
20. You need to store financial transactions with strict consistency. Is MongoDB suitable?
21. Your application has rapidly changing schema requirements. Which database fits better?

---

## 5.2 CRUD Operations

### ✅ Important Topics
- [ ] insertOne(), insertMany()
- [ ] find(), findOne()
- [ ] updateOne(), updateMany()
- [ ] deleteOne(), deleteMany()
- [ ] replaceOne()
- [ ] findOneAndUpdate(), findOneAndDelete()
- [ ] bulkWrite()
- [ ] Upsert
- [ ] Update operators ($set, $unset, $push, $pull, $addToSet, $inc, $min, $max, $rename)
- [ ] Query operators ($eq, $ne, $gt, $gte, $lt, $lte, $in, $nin, $and, $or, $not, $exists, $regex)
- [ ] Projection
- [ ] Cursors
- [ ] sort(), limit(), skip()
- [ ] countDocuments(), estimatedDocumentCount()
- [ ] distinct()

### 📋 Interview Questions
1. How do you insert a document in MongoDB?
2. What is the difference between `insertOne()` and `insertMany()`?
3. How do you find documents in MongoDB?
4. What is the difference between `find()` and `findOne()`?
5. How do you update a document? What is the difference between `updateOne()` and `updateMany()`?
6. What is the difference between `updateOne()` and `replaceOne()`?
7. What is `findOneAndUpdate()`? How is it different from `updateOne()`?
8. How do you delete documents?
9. What is an upsert? When would you use it?
10. What is the `$set` operator?
11. What is the `$push` operator? How is it different from `$addToSet`?
12. What is the `$pull` operator?
13. What is the `$inc` operator?
14. What are comparison operators in MongoDB? ($gt, $gte, $lt, $lte, $eq, $ne)
15. What are logical operators? ($and, $or, $not, $nor)
16. What is the `$in` operator?
17. What is the `$exists` operator?
18. What is the `$regex` operator?
19. What is projection in MongoDB?
20. How do you implement pagination using `skip()` and `limit()`?
21. What are the problems with `skip()` for large datasets? What is cursor-based pagination?
22. What is a cursor in MongoDB?
23. What is `bulkWrite()`? When would you use it?
24. How do you count documents in a collection?
25. How do you get distinct values of a field?

### 💻 Practical Query Questions
26. Find all users whose age is greater than 25 and city is "Mumbai".
27. Find all products with price between 100 and 500.
28. Update the status of all orders placed before a certain date.
29. Remove a specific element from an array field.
30. Add a new tag to an array field only if it doesn't already exist.
31. Increment the view count of a blog post by 1.
32. Find all users whose name starts with "A" (case-insensitive).
33. Find the top 10 highest-priced products.
34. Find users who have at least one order.
35. Find all documents where a specific field does not exist.

---

## 5.3 Aggregation Pipeline

### ✅ Important Topics
- [ ] Aggregation pipeline concept
- [ ] Pipeline stages ($match, $group, $project, $sort, $limit, $skip, $unwind, $lookup, $addFields, $count, $facet, $bucket, $merge, $out)
- [ ] Accumulator operators ($sum, $avg, $min, $max, $first, $last, $push, $addToSet)
- [ ] $lookup (join)
- [ ] $unwind
- [ ] $facet (multiple pipelines)
- [ ] $bucket and $bucketAuto
- [ ] Pipeline optimization

### 📋 Interview Questions
1. What is the aggregation pipeline in MongoDB?
2. What is the difference between `find()` and `aggregate()`?
3. What is the `$match` stage?
4. What is the `$group` stage? What are accumulator operators?
5. What is `$project`?
6. What is `$unwind`? When do you use it?
7. What is `$lookup`? How do you perform joins in MongoDB?
8. What is the difference between `$lookup` and embedding?
9. What is `$addFields`?
10. What is `$facet`? When would you use it?
11. What is `$bucket`?
12. What is the order of stages in the aggregation pipeline? Does it matter?
13. How do you optimize an aggregation pipeline?
14. What is `$merge` vs `$out`?
15. Can you use indexes in aggregation pipelines?

### 💻 Practical Aggregation Questions
16. Find the total number of orders per customer.
17. Find the average price of products in each category.
18. Find the top 5 customers by total order amount.
19. Unwind an array of tags and count the frequency of each tag.
20. Perform a join between orders and users collections.
21. Group users by age range (18-25, 26-35, 36-45, 45+).
22. Find the month with the highest number of orders.
23. Calculate the running total of sales per month.
24. Find products that are out of stock (quantity = 0) in each category.
25. Create a paginated aggregation with total count.

---

## 5.4 Indexes

### ✅ Important Topics
- [ ] What are indexes
- [ ] Single field index
- [ ] Compound index
- [ ] Multikey index (array fields)
- [ ] Text index
- [ ] Geospatial index (2dsphere)
- [ ] Unique index
- [ ] Sparse index
- [ ] Partial index
- [ ] TTL index
- [ ] Covered queries
- [ ] explain() for query analysis
- [ ] Index performance impact
- [ ] When to create and when NOT to create indexes

### 📋 Interview Questions
1. What are indexes in MongoDB? Why are they important?
2. What is the default index in MongoDB?
3. How do you create an index?
4. What is a compound index? How does the field order matter?
5. What is a multikey index?
6. What is a text index? How do you use it for full-text search?
7. What is a unique index?
8. What is a sparse index? When would you use it?
9. What is a TTL index? Give a use case.
10. What is a partial index?
11. What is a covered query?
12. How do you analyze query performance? What is `explain()`?
13. What is the ESR rule (Equality, Sort, Range)?
14. What are the disadvantages of indexes?
15. When should you NOT create an index?
16. How many indexes can a collection have?
17. What happens to indexes when you drop a collection?
18. What is index intersection?

### 🎯 Scenario Based Questions
19. Your query on a collection with 10 million documents is slow. How do you optimize it?
20. You have a query that filters by `status` and sorts by `createdAt`. What index would you create?
21. You need to automatically delete documents after 30 days. How do you do it?
22. You need to search through blog post content. What type of index do you use?

---

## 5.5 Schema Design

### ✅ Important Topics
- [ ] Schema-less vs Schema validation
- [ ] Mongoose schema and models
- [ ] Data types in Mongoose
- [ ] Schema options (timestamps, toJSON, toObject)
- [ ] Virtuals
- [ ] Instance methods
- [ ] Static methods
- [ ] Middleware (pre, post hooks)
- [ ] Validators (built-in and custom)
- [ ] Schema design patterns
- [ ] One-to-One, One-to-Many, Many-to-Many relationships

### 📋 Interview Questions
1. What is a Mongoose schema?
2. What is the difference between a schema and a model in Mongoose?
3. What data types does Mongoose support?
4. What is `timestamps: true` in a schema?
5. What are virtuals in Mongoose? Give an example.
6. What are instance methods vs static methods in Mongoose?
7. What is middleware (hooks) in Mongoose? What types exist?
8. What is the difference between `pre('save')` and `pre('validate')`?
9. How do you implement custom validation in Mongoose?
10. What are built-in validators in Mongoose?
11. How do you handle one-to-one relationships in MongoDB?
12. How do you handle one-to-many relationships?
13. How do you handle many-to-many relationships?
14. What are the schema design best practices for MongoDB?

---

## 5.6 Embedding vs Referencing

### ✅ Important Topics
- [ ] Embedded documents (subdocuments)
- [ ] Referenced documents (normalization)
- [ ] When to embed vs when to reference
- [ ] populate() in Mongoose
- [ ] Denormalization
- [ ] Data duplication tradeoffs
- [ ] 16MB document size limit

### 📋 Interview Questions
1. What is embedding in MongoDB?
2. What is referencing in MongoDB?
3. What is the difference between embedding and referencing?
4. When should you embed documents?
5. When should you reference documents?
6. What is `populate()` in Mongoose? How does it work internally?
7. What is the performance impact of `populate()`?
8. What is denormalization? What are its advantages and disadvantages?
9. What is the 16MB document size limit? How does it affect schema design?
10. Can you partially populate referenced documents?
11. What are the rules of thumb for embedding vs referencing?

### 🎯 Scenario Based Questions
12. You have a blog application. Should you embed comments in the blog post or reference them?
13. You have an e-commerce app. How would you model products and categories?
14. A user can have thousands of orders. Would you embed orders in the user document?
15. How would you model a social media app with users, posts, comments, and likes?
16. Design the MongoDB schema for a food delivery application.

---

## 5.7 Transactions

### ✅ Important Topics
- [ ] ACID properties in MongoDB
- [ ] Multi-document transactions
- [ ] Sessions
- [ ] Transaction lifecycle
- [ ] Write concerns
- [ ] Read concerns
- [ ] Read preferences
- [ ] When to use transactions

### 📋 Interview Questions
1. Does MongoDB support transactions?
2. What are ACID properties? Does MongoDB follow them?
3. What are multi-document transactions?
4. How do you implement transactions in Mongoose?
5. What is a session in MongoDB transactions?
6. What are write concerns? What does `w: 'majority'` mean?
7. What are read concerns?
8. What are read preferences?
9. When should you use transactions in MongoDB?
10. What is the performance impact of transactions?
11. What happens if a transaction fails?
12. Can you use transactions in standalone MongoDB? (No, need replica set)

### 💻 Coding Questions
13. Implement a money transfer between two accounts using MongoDB transactions.
14. Implement order creation that updates inventory atomically.

---

## 5.8 Sharding

### ✅ Important Topics
- [ ] What is sharding
- [ ] Shard key
- [ ] Chunks
- [ ] Balancer
- [ ] Range-based sharding
- [ ] Hash-based sharding
- [ ] Config servers
- [ ] mongos router
- [ ] When to shard

### 📋 Interview Questions
1. What is sharding in MongoDB?
2. Why is sharding needed?
3. What is a shard key? How do you choose it?
4. What is the difference between range-based and hash-based sharding?
5. What is a chunk in MongoDB sharding?
6. What is the balancer?
7. What are config servers?
8. What is `mongos`?
9. What are the characteristics of a good shard key?
10. Can you change the shard key after sharding?
11. What is the difference between sharding and replication?
12. When should you shard your MongoDB cluster?

---

## 5.9 Replication

### ✅ Important Topics
- [ ] Replica sets
- [ ] Primary and Secondary nodes
- [ ] Arbiter
- [ ] Automatic failover
- [ ] Election process
- [ ] Oplog (operation log)
- [ ] Read preferences with replica sets
- [ ] Write concerns with replica sets

### 📋 Interview Questions
1. What is replication in MongoDB?
2. What is a replica set?
3. What is the minimum number of nodes in a replica set?
4. What is the role of the primary node?
5. What is the role of secondary nodes?
6. What is an arbiter?
7. What happens when the primary node goes down?
8. What is the election process?
9. What is the oplog?
10. How does replication ensure data consistency?
11. What is the difference between replication and sharding?
12. Can you read from secondary nodes? What are the tradeoffs?

---

## 5.10 MongoDB Atlas

### ✅ Important Topics
- [ ] Atlas setup and configuration
- [ ] Clusters (shared, dedicated, serverless)
- [ ] Network access and IP whitelisting
- [ ] Database users and roles
- [ ] Atlas Search
- [ ] Atlas Data API
- [ ] Monitoring and alerts
- [ ] Backup and restore
- [ ] Connection string configuration

### 📋 Interview Questions
1. What is MongoDB Atlas?
2. How do you create a cluster on Atlas?
3. What is IP whitelisting? Why is it important?
4. How do you create database users in Atlas?
5. What is Atlas Search?
6. How do you monitor your MongoDB Atlas cluster?
7. How do you backup and restore data in Atlas?
8. What are the different cluster tiers in Atlas?
9. What is the Atlas Data API?
10. How do you connect a Node.js application to MongoDB Atlas?

---

## 5.11 MongoDB Optimization

### ✅ Important Topics
- [ ] Query optimization using explain()
- [ ] Index optimization
- [ ] Aggregation pipeline optimization
- [ ] Schema design optimization
- [ ] Projection to reduce data transfer
- [ ] Connection pooling
- [ ] Read/Write concerns tuning
- [ ] Avoiding N+1 queries
- [ ] Caching strategies

### 📋 Interview Questions
1. How do you optimize slow MongoDB queries?
2. What does `explain()` tell you?
3. What is a collection scan vs index scan?
4. How do you avoid the N+1 query problem with Mongoose?
5. What is lean() in Mongoose? How does it improve performance?
6. How does projection improve query performance?
7. What is the impact of large document sizes on performance?
8. How do you optimize aggregation pipelines?
9. What are the best practices for MongoDB performance?
10. How do you monitor MongoDB performance?

### 🎯 Scenario Based Questions
11. A query that was fast with 1000 documents is now slow with 10 million documents. What do you check?
12. Your MongoDB cluster has high CPU usage. What could be causing it?
13. Read operations are slow. Write operations are fine. What could be the issue?
14. You need to store 100 million documents. How do you plan your MongoDB architecture?

---

### 🎯 What Interviewer Expects (MongoDB)
- [ ] Understanding of when to use MongoDB vs SQL
- [ ] Ability to design proper schemas (embedding vs referencing)
- [ ] Knowledge of CRUD operations and query operators
- [ ] Understanding of aggregation pipeline
- [ ] Knowledge of indexing strategies
- [ ] Awareness of transactions and when to use them
- [ ] Understanding of replication and sharding concepts
- [ ] Ability to optimize queries

### ❌ Common Mistakes (MongoDB)
- [ ] Not creating indexes on frequently queried fields
- [ ] Using `skip()` for pagination on large collections
- [ ] Over-embedding leading to documents exceeding 16MB
- [ ] Not using `lean()` when you don't need Mongoose document features
- [ ] Using `populate()` excessively (N+1 problem)
- [ ] Not using projection to limit returned fields
- [ ] Not handling `unique` index violations
- [ ] Not using transactions when atomic operations are needed
- [ ] Choosing the wrong shard key
- [ ] Not understanding the difference between `updateOne()` and `replaceOne()`

---

> **📌 SECTION 5 COMPLETE — MongoDB**

---
