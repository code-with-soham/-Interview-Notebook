# ═══════════════════════════════════════════════════════
# SECTION 4: NODE.JS (COMPLETE)
# ═══════════════════════════════════════════════════════

---

## 4.1 Node.js Fundamentals

### ✅ Important Topics
- [ ] What is Node.js
- [ ] V8 Engine
- [ ] Single-threaded architecture
- [ ] Non-blocking I/O
- [ ] Node.js vs Browser JavaScript
- [ ] Global objects (process, __dirname, __filename, Buffer, global)
- [ ] REPL
- [ ] Node.js architecture
- [ ] CommonJS vs ES Modules in Node
- [ ] npm vs yarn vs pnpm
- [ ] package.json and package-lock.json
- [ ] Semantic versioning
- [ ] npx
- [ ] .env files and dotenv
- [ ] Node.js versions and LTS

### 📋 Interview Questions
1. What is Node.js? Is it a language, framework, or runtime?
2. Why is Node.js called single-threaded?
3. What is the V8 engine?
4. What is non-blocking I/O? Why is it important?
5. What is the difference between Node.js and browser JavaScript?
6. What are global objects in Node.js?
7. What is the `process` object? What are `process.env`, `process.argv`, `process.exit()`?
8. What is the difference between `require` and `import` in Node.js?
9. What is `package.json`? What are its important fields?
10. What is `package-lock.json`? Why is it important?
11. What is semantic versioning? What does `^` and `~` mean in versions?
12. What is the difference between `npm install` and `npm ci`?
13. What are `devDependencies` vs `dependencies`?
14. What is `npx`? How is it different from `npm`?
15. What is the difference between `npm` and `yarn`?
16. How does Node.js handle concurrent requests if it's single-threaded?
17. What are the advantages and disadvantages of Node.js?
18. When should you NOT use Node.js?
19. What is the difference between Node.js and Express.js?
20. What is the `module` object in Node.js?

### 🎯 Scenario Based Questions
21. You need to build a real-time chat application. Why would you choose Node.js?
22. You need to do heavy image processing. Is Node.js the right choice? Why/why not?
23. Your Node.js app is consuming too much memory. How would you debug it?

---

## 4.2 Node.js Event Loop

### ✅ Important Topics
- [ ] Event Loop architecture
- [ ] Event Loop phases (Timers, Pending Callbacks, Idle/Prepare, Poll, Check, Close Callbacks)
- [ ] process.nextTick()
- [ ] setImmediate() vs setTimeout()
- [ ] Microtasks vs Macrotasks in Node.js
- [ ] Event-driven architecture
- [ ] Non-blocking vs Blocking code
- [ ] Thread pool (libuv)

### 📋 Interview Questions
1. What is the Event Loop in Node.js?
2. How is the Node.js Event Loop different from the browser Event Loop?
3. What are the phases of the Node.js Event Loop?
4. What happens in the Timer phase?
5. What happens in the Poll phase?
6. What happens in the Check phase?
7. What is `process.nextTick()`? When should you use it?
8. What is the difference between `process.nextTick()` and `setImmediate()`?
9. What is the difference between `setImmediate()` and `setTimeout(fn, 0)`?
10. What is the priority order of `process.nextTick()`, `Promise.then()`, `setTimeout()`, and `setImmediate()`?
11. Can the Event Loop be blocked? How?
12. What happens if you block the Event Loop?
13. How do you detect Event Loop blocking?

### 🖥️ Output Based Questions
14. What is the output?
```js
console.log('start');
setTimeout(() => console.log('timeout'), 0);
setImmediate(() => console.log('immediate'));
process.nextTick(() => console.log('nextTick'));
Promise.resolve().then(() => console.log('promise'));
console.log('end');
```

15. What is the output?
```js
setImmediate(() => console.log('1'));
setTimeout(() => console.log('2'), 0);
```

16. What is the output?
```js
const fs = require('fs');
fs.readFile(__filename, () => {
  setTimeout(() => console.log('timeout'));
  setImmediate(() => console.log('immediate'));
});
```

17. What is the output?
```js
process.nextTick(() => console.log('nextTick 1'));
Promise.resolve().then(() => console.log('promise 1'));
process.nextTick(() => console.log('nextTick 2'));
Promise.resolve().then(() => console.log('promise 2'));
```

18. What is the output?
```js
setTimeout(() => {
  console.log('timeout 1');
  process.nextTick(() => console.log('nextTick inside timeout'));
}, 0);
setTimeout(() => {
  console.log('timeout 2');
}, 0);
```

---

## 4.3 libuv

### ✅ Important Topics
- [ ] What is libuv
- [ ] Thread pool (default 4 threads)
- [ ] UV_THREADPOOL_SIZE
- [ ] Async I/O operations
- [ ] libuv and the Event Loop relationship
- [ ] OS-level async (epoll, kqueue, IOCP)
- [ ] Which operations use the thread pool

### 📋 Interview Questions
1. What is libuv? What role does it play in Node.js?
2. What is the thread pool in libuv?
3. What is the default size of the libuv thread pool?
4. How do you change the thread pool size?
5. Which operations use the thread pool? Which don't?
6. What is the difference between the Event Loop and the thread pool?
7. How does libuv handle file system operations?
8. How does libuv handle network operations?
9. What is the relationship between V8, libuv, and Node.js?
10. What happens when the thread pool is exhausted?

---

## 4.4 Streams

### ✅ Important Topics
- [ ] Readable streams
- [ ] Writable streams
- [ ] Duplex streams
- [ ] Transform streams
- [ ] Stream modes (flowing, paused)
- [ ] Piping
- [ ] Backpressure
- [ ] Stream events (data, end, error, finish, drain)
- [ ] Creating custom streams
- [ ] Stream vs Buffer

### 📋 Interview Questions
1. What are streams in Node.js?
2. What are the types of streams?
3. What is a Readable stream? Give examples.
4. What is a Writable stream? Give examples.
5. What is a Duplex stream? Give examples.
6. What is a Transform stream? Give examples.
7. What is piping? How do you pipe streams?
8. What is backpressure? How do you handle it?
9. What are the events emitted by a Readable stream?
10. What is the difference between flowing mode and paused mode?
11. How do you create a custom Readable stream?
12. Why are streams more memory-efficient than reading entire files?
13. What is `pipeline()` and how is it different from `pipe()`?

### 💻 Coding Questions
14. Read a large file using streams and write it to another file.
15. Create a Transform stream that converts text to uppercase.
16. Implement a custom Readable stream that generates random numbers.
17. Use streams to compress a file with gzip.
18. Read a CSV file line-by-line using streams.

### 🎯 Scenario Based Questions
19. You need to process a 10GB log file. How would you do it in Node.js?
20. You need to stream video content to a client. How would you implement it?
21. Your application is running out of memory when processing large files. What's the solution?

---

## 4.5 Buffers

### ✅ Important Topics
- [ ] What is a Buffer
- [ ] Buffer creation (Buffer.alloc, Buffer.from)
- [ ] Buffer encoding (utf-8, base64, hex)
- [ ] Buffer vs String
- [ ] Buffer concatenation
- [ ] Buffer and streams relationship
- [ ] Binary data handling

### 📋 Interview Questions
1. What is a Buffer in Node.js?
2. Why do we need Buffers in Node.js?
3. What is the difference between `Buffer.alloc()` and `Buffer.allocUnsafe()`?
4. How do you create a Buffer from a string?
5. How do you convert a Buffer to a string?
6. What is the relationship between Buffers and Streams?
7. What is the default encoding of a Buffer?
8. Can you resize a Buffer after creation?
9. What is `Buffer.concat()`?
10. How do you handle binary data in Node.js?

---

## 4.6 Cluster Module

### ✅ Important Topics
- [ ] What is clustering
- [ ] Master-Worker pattern
- [ ] cluster.fork()
- [ ] Load balancing (round-robin)
- [ ] IPC (Inter-Process Communication)
- [ ] Scaling Node.js applications
- [ ] PM2 and clustering
- [ ] Cluster vs Worker Threads

### 📋 Interview Questions
1. What is the Cluster module in Node.js?
2. How does clustering help with performance?
3. What is the master-worker pattern in Node.js clustering?
4. How does the cluster module distribute incoming requests?
5. What is round-robin load balancing?
6. What is IPC? How do master and worker processes communicate?
7. How many workers should you create?
8. What happens when a worker process crashes?
9. What is PM2? How does it relate to clustering?
10. What is the difference between `cluster.isMaster` and `cluster.isPrimary`?

### 💻 Coding Questions
11. Create a basic Node.js cluster setup with multiple workers.
12. Implement a cluster setup that automatically restarts crashed workers.
13. Implement load balancing across multiple CPU cores.

---

## 4.7 Worker Threads

### ✅ Important Topics
- [ ] What are Worker Threads
- [ ] Worker Threads vs Cluster
- [ ] Worker Threads vs Child Processes
- [ ] SharedArrayBuffer
- [ ] MessagePort
- [ ] Use cases for Worker Threads
- [ ] CPU-intensive tasks

### 📋 Interview Questions
1. What are Worker Threads in Node.js?
2. What is the difference between Worker Threads and the Cluster module?
3. What is the difference between Worker Threads and Child Processes?
4. When should you use Worker Threads?
5. How do Worker Threads communicate with the main thread?
6. What is `SharedArrayBuffer`?
7. What is `MessagePort`?
8. Can Worker Threads share memory?
9. What types of tasks are suitable for Worker Threads?
10. Are Worker Threads truly parallel in Node.js?

### 💻 Coding Questions
11. Create a Worker Thread that computes the Fibonacci of a large number.
12. Implement a task queue using Worker Threads.

---

## 4.8 Express.js

### ✅ Important Topics
- [ ] Express basics
- [ ] Routing (GET, POST, PUT, PATCH, DELETE)
- [ ] Route parameters and query strings
- [ ] Request and Response objects
- [ ] Express Router
- [ ] Static files (express.static)
- [ ] Template engines (EJS, Pug)
- [ ] Error handling in Express
- [ ] Express application structure

### 📋 Interview Questions
1. What is Express.js? Why is it used?
2. What is the difference between Express.js and Node.js?
3. How do you create a basic Express server?
4. What is routing in Express?
5. What is the difference between `app.get()` and `app.use()`?
6. What are route parameters? How do you access them?
7. What are query parameters? How do you access them?
8. What is the difference between `req.params`, `req.query`, and `req.body`?
9. What is `express.Router()`? Why is it used?
10. How do you serve static files in Express?
11. What is `express.json()` and `express.urlencoded()`?
12. How do you handle 404 errors in Express?
13. How do you handle errors globally in Express?
14. What is the request-response lifecycle in Express?
15. What is the difference between `res.send()`, `res.json()`, and `res.end()`?
16. What is the difference between `PUT` and `PATCH`?
17. How do you group routes in Express?
18. What is the difference between `app.route()` and `express.Router()`?

### 💻 Coding Questions
19. Create a basic Express server with CRUD routes.
20. Implement a route that handles file uploads.
21. Create a modular route structure using Express Router.
22. Implement a global error handler middleware.

---

## 4.9 Middleware

### ✅ Important Topics
- [ ] What is middleware
- [ ] Middleware execution order
- [ ] next() function
- [ ] Application-level middleware
- [ ] Router-level middleware
- [ ] Built-in middleware (express.json, express.static)
- [ ] Third-party middleware (cors, helmet, morgan)
- [ ] Error-handling middleware
- [ ] Custom middleware
- [ ] Middleware chaining

### 📋 Interview Questions
1. What is middleware in Express?
2. How does middleware work in Express?
3. What is the `next()` function? What happens if you don't call it?
4. What is the order of middleware execution?
5. What are the types of middleware in Express?
6. What is application-level middleware vs router-level middleware?
7. What are built-in middleware in Express?
8. What is `cors` middleware? Why is it needed?
9. What is `helmet` middleware? What does it do?
10. What is `morgan` middleware?
11. How do you create custom middleware?
12. What is error-handling middleware? How is it different from regular middleware?
13. How many arguments does error-handling middleware have?
14. Can middleware modify the request and response objects?
15. How do you apply middleware to specific routes only?

### 💻 Coding Questions
16. Create a logging middleware that logs the request method, URL, and timestamp.
17. Create an authentication middleware that checks for a valid JWT token.
18. Create a rate-limiting middleware from scratch.
19. Create a request validation middleware.
20. Create a middleware that measures response time.

### 🎯 Scenario Based Questions
21. You have middleware A, B, and C. A calls next(), B does not. What happens to C?
22. You need to add CORS support to your API. How do you do it?
23. You want to log every request and its response time. How do you implement this?

---

## 4.10 Authentication & Authorization

### ✅ Important Topics
- [ ] Authentication vs Authorization
- [ ] Session-based authentication
- [ ] Token-based authentication (JWT)
- [ ] OAuth 2.0
- [ ] Passport.js
- [ ] bcrypt for password hashing
- [ ] Salt and hashing
- [ ] Refresh tokens
- [ ] Role-based access control (RBAC)
- [ ] API Key authentication

### 📋 Interview Questions
1. What is the difference between authentication and authorization?
2. What is session-based authentication? How does it work?
3. What is token-based authentication? How does it work?
4. What is the difference between session-based and token-based authentication?
5. When would you use session-based over token-based authentication?
6. What is OAuth 2.0? Explain the flow.
7. What is Passport.js? What strategies does it support?
8. How do you hash passwords in Node.js?
9. What is a salt? Why is it important?
10. What is the difference between hashing and encryption?
11. What is bcrypt? Why is it preferred for password hashing?
12. What is RBAC? How do you implement it?
13. How do you implement "forgot password" functionality?
14. What is multi-factor authentication (MFA)?
15. How do you implement social login (Google, GitHub)?

---

## 4.11 JWT (JSON Web Token)

### ✅ Important Topics
- [ ] JWT structure (Header, Payload, Signature)
- [ ] JWT creation and verification
- [ ] Access tokens and Refresh tokens
- [ ] JWT expiration
- [ ] JWT storage (cookies vs localStorage)
- [ ] JWT vs Session
- [ ] JWT security concerns
- [ ] Token blacklisting/revocation

### 📋 Interview Questions
1. What is JWT? What does it stand for?
2. What are the three parts of a JWT?
3. What is in the Header of a JWT?
4. What is in the Payload of a JWT?
5. What is the Signature of a JWT? How is it created?
6. Is JWT encrypted?
7. Can you read the data inside a JWT without the secret?
8. What is the difference between an access token and a refresh token?
9. Why do we need refresh tokens?
10. How do you implement token refresh in Node.js?
11. Where should you store JWT tokens? Why?
12. What are the security risks of JWT?
13. How do you invalidate/revoke a JWT?
14. What is token blacklisting?
15. What happens if someone steals your JWT?
16. What is the difference between JWT and session-based authentication?
17. What is the `jsonwebtoken` library? How do you use it?
18. How do you set token expiration?
19. What is the difference between symmetric and asymmetric JWT signing?
20. What is the `iss`, `sub`, `exp`, `iat` in JWT claims?

### 💻 Coding Questions
21. Implement JWT authentication (sign, verify, middleware).
22. Implement a refresh token rotation flow.
23. Implement JWT with HTTP-only cookies.
24. Create a middleware that validates JWT and attaches user to request.

---

## 4.12 Cookies in Node.js

### ✅ Important Topics
- [ ] Setting cookies (res.cookie)
- [ ] Reading cookies (req.cookies with cookie-parser)
- [ ] Cookie attributes (httpOnly, secure, sameSite, path, domain, maxAge, expires)
- [ ] Signed cookies
- [ ] Cookie vs Session vs JWT
- [ ] Cookie security

### 📋 Interview Questions
1. How do you set a cookie in Express?
2. How do you read cookies in Express?
3. What is `cookie-parser` middleware?
4. What is the `HttpOnly` flag? Why is it important?
5. What is the `Secure` flag?
6. What is the `SameSite` attribute? What are its values?
7. What are signed cookies?
8. What is the difference between `maxAge` and `expires`?
9. How do you delete a cookie?
10. What is the maximum size of a cookie?

---

## 4.13 MVC Architecture

### ✅ Important Topics
- [ ] Model-View-Controller pattern
- [ ] Models (data layer)
- [ ] Views (presentation layer)
- [ ] Controllers (business logic)
- [ ] Routes
- [ ] Services layer
- [ ] Repository pattern
- [ ] Separation of concerns
- [ ] Folder structure for MVC

### 📋 Interview Questions
1. What is the MVC architecture?
2. What is the role of Model, View, and Controller?
3. How do you implement MVC in an Express.js application?
4. What is the Service layer? Where does it fit in MVC?
5. What is the Repository pattern?
6. What is the difference between a Controller and a Service?
7. Why is MVC important for large-scale applications?
8. What is the folder structure for an MVC-based Express app?
9. What is the difference between MVC and MVVM?
10. How do you handle business logic in MVC — in the Controller or Service?

### 🎯 Scenario Based Questions
11. You have API logic mixed with database queries in your routes. How do you refactor using MVC?
12. Design the folder structure for a MERN e-commerce application using MVC.
13. Where should input validation happen in MVC — routes, controller, or model?

---

## 4.14 REST API Design

### ✅ Important Topics
- [ ] REST principles
- [ ] HTTP methods (GET, POST, PUT, PATCH, DELETE)
- [ ] Status codes
- [ ] URL naming conventions
- [ ] Versioning
- [ ] Pagination, Filtering, Sorting
- [ ] HATEOAS
- [ ] Idempotency
- [ ] Request/Response formats
- [ ] API documentation (Swagger/OpenAPI)

### 📋 Interview Questions
1. What is a RESTful API?
2. What are the REST principles/constraints?
3. What is the difference between REST and SOAP?
4. What is the difference between REST and GraphQL?
5. What are the HTTP methods and their use cases?
6. What is the difference between PUT and PATCH?
7. What is the difference between POST and PUT?
8. What is idempotency? Which HTTP methods are idempotent?
9. What are common HTTP status codes and their meanings? (200, 201, 204, 400, 401, 403, 404, 409, 500)
10. What is the correct URL naming convention for REST APIs?
11. How do you implement pagination in a REST API?
12. How do you implement filtering and sorting?
13. What is API versioning? What strategies exist?
14. What is HATEOAS?
15. How do you document a REST API?

---

## 4.15 Rate Limiting

### ✅ Important Topics
- [ ] What is rate limiting
- [ ] Token bucket algorithm
- [ ] Sliding window algorithm
- [ ] Fixed window algorithm
- [ ] express-rate-limit
- [ ] Rate limiting by IP, user, API key
- [ ] DDoS protection
- [ ] Rate limit headers (X-RateLimit-Remaining)

### 📋 Interview Questions
1. What is rate limiting? Why is it needed?
2. What are the different rate limiting algorithms?
3. What is the token bucket algorithm?
4. What is the sliding window algorithm?
5. How do you implement rate limiting in Express?
6. How do you rate limit by IP vs by user?
7. What is the `express-rate-limit` package?
8. What HTTP status code do you return when rate limit is exceeded?
9. How do you implement rate limiting in a distributed system?
10. What is the difference between rate limiting and throttling?

### 💻 Coding Questions
11. Implement a basic rate limiter middleware from scratch.
12. Implement rate limiting using Redis for distributed systems.

---

## 4.16 Validation

### ✅ Important Topics
- [ ] Input validation
- [ ] Joi library
- [ ] express-validator
- [ ] Zod
- [ ] Schema validation
- [ ] Sanitization
- [ ] Request body validation
- [ ] Query parameter validation
- [ ] Custom validators

### 📋 Interview Questions
1. Why is input validation important?
2. Where should validation happen — client-side, server-side, or both?
3. What is schema validation?
4. What is the difference between Joi, express-validator, and Zod?
5. How do you validate request body, query params, and route params?
6. What is sanitization? How is it different from validation?
7. How do you create custom validators?
8. How do you return validation errors to the client?
9. What is the difference between validation and authentication middleware?

### 💻 Coding Questions
10. Create a validation middleware using Joi for a user registration endpoint.
11. Implement request validation using Zod.
12. Create a reusable validation middleware factory.

---

## 4.17 Error Handling

### ✅ Important Topics
- [ ] try/catch
- [ ] Error types (operational vs programming errors)
- [ ] Global error handler middleware
- [ ] Async error handling
- [ ] Custom error classes
- [ ] Uncaught exceptions
- [ ] Unhandled promise rejections
- [ ] Error logging
- [ ] Error response format
- [ ] process.on('uncaughtException') and process.on('unhandledRejection')

### 📋 Interview Questions
1. How do you handle errors in Express?
2. What is the difference between operational and programming errors?
3. How do you create a global error handler in Express?
4. How do you handle async errors in Express?
5. Why is wrapping async route handlers important?
6. What is a custom error class? How do you create one?
7. What is `process.on('uncaughtException')`? When does it fire?
8. What is `process.on('unhandledRejection')`?
9. Should you crash the process on uncaught exceptions? Why?
10. How do you create a consistent error response format?
11. How do you handle 404 errors in Express?
12. What is the `express-async-errors` package?

### 💻 Coding Questions
13. Create a custom `AppError` class with status code and message.
14. Create an async wrapper (`catchAsync`) to handle async errors.
15. Implement a global error handling middleware.
16. Create different error classes (NotFoundError, ValidationError, AuthenticationError).

---

## 4.18 Logging

### ✅ Important Topics
- [ ] Console logging
- [ ] Winston logger
- [ ] Morgan HTTP logger
- [ ] Pino logger
- [ ] Log levels (error, warn, info, debug)
- [ ] Log formatting
- [ ] Log rotation
- [ ] Structured logging
- [ ] Logging in production

### 📋 Interview Questions
1. Why is logging important in production applications?
2. What are log levels? Name them in order.
3. What is Winston? How do you use it?
4. What is Morgan? When do you use it?
5. What is the difference between Morgan and Winston?
6. What is structured logging?
7. What is log rotation? Why is it needed?
8. What should you NOT log? (passwords, tokens, PII)
9. How do you implement logging in a production Express app?
10. What is the difference between `console.log()` and a proper logger?

---

## 4.19 Scalability

### ✅ Important Topics
- [ ] Horizontal scaling vs Vertical scaling
- [ ] Clustering
- [ ] Load balancing
- [ ] Reverse proxy (Nginx)
- [ ] Caching (Redis)
- [ ] Database optimization
- [ ] Connection pooling
- [ ] Microservices
- [ ] Message queues (RabbitMQ, Kafka)
- [ ] Stateless architecture

### 📋 Interview Questions
1. How do you scale a Node.js application?
2. What is the difference between horizontal and vertical scaling?
3. How does clustering help scale Node.js?
4. What is a reverse proxy? Why use Nginx with Node.js?
5. How do you implement caching in Node.js?
6. What is Redis? How do you use it for caching?
7. What is connection pooling?
8. Why should a Node.js application be stateless?
9. How do you handle sessions in a scaled Node.js application?
10. What is a message queue? When would you use one?
11. How do you handle file uploads in a scaled environment?
12. What is the difference between monolith and microservices?

### 🎯 Scenario Based Questions
13. Your Node.js API handles 100 requests/second but needs to handle 10,000. What do you do?
14. Your API response time is 2 seconds. How do you reduce it?
15. You deploy your Node.js app on 5 servers. How do you handle user sessions?

---

## 4.20 Security

### ✅ Important Topics
- [ ] Helmet.js
- [ ] CORS
- [ ] Input sanitization
- [ ] SQL/NoSQL injection
- [ ] XSS prevention
- [ ] CSRF protection
- [ ] Rate limiting
- [ ] HTTPS
- [ ] Environment variables (.env)
- [ ] Dependency vulnerabilities (npm audit)
- [ ] HTTP security headers
- [ ] Data validation and sanitization

### 📋 Interview Questions
1. How do you secure a Node.js/Express application?
2. What is Helmet.js? What security headers does it set?
3. How do you prevent NoSQL injection in MongoDB?
4. How do you prevent XSS in Express?
5. How do you implement CORS in Express?
6. What is CSRF? How do you prevent it in Express?
7. Why should you store secrets in environment variables?
8. What is `npm audit`? How do you use it?
9. How do you implement HTTPS in Node.js?
10. What are HTTP security headers?
11. How do you sanitize user input in Express?
12. What is parameterized/prepared statements?
13. How do you handle file upload security?
14. What is the principle of least privilege?
15. How do you prevent brute force attacks?

---

## 4.21 Performance Optimization

### ✅ Important Topics
- [ ] Profiling Node.js applications
- [ ] Memory leaks detection
- [ ] Event Loop monitoring
- [ ] Caching strategies
- [ ] Database query optimization
- [ ] Compression (gzip)
- [ ] Connection pooling
- [ ] Lazy loading
- [ ] Avoiding synchronous operations
- [ ] Using streams for large data
- [ ] CDN for static assets
- [ ] PM2 for process management

### 📋 Interview Questions
1. How do you profile a Node.js application?
2. How do you detect and fix memory leaks in Node.js?
3. What is `--inspect` flag? How do you use Chrome DevTools for Node.js?
4. How do you enable gzip compression in Express?
5. What is PM2? What features does it provide?
6. How do you handle CPU-intensive tasks without blocking the Event Loop?
7. What are the performance differences between reading files synchronously vs asynchronously?
8. How do you optimize database queries in a Node.js application?
9. What is response caching? How do you implement it?
10. How do you monitor a Node.js application in production?
11. What is the `heapdump` module?
12. What tools do you use for load testing? (Artillery, k6, Apache Benchmark)
13. How do you implement graceful shutdown in Node.js?

### 💻 Coding Questions
14. Implement gzip compression middleware in Express.
15. Implement a simple in-memory cache with TTL.
16. Create a graceful shutdown handler for your Express server.
17. Implement connection pooling for MongoDB.

---

## 4.22 File System (fs) Module

### ✅ Important Topics
- [ ] Reading files (readFile, readFileSync, createReadStream)
- [ ] Writing files (writeFile, writeFileSync, createWriteStream)
- [ ] Appending files
- [ ] Deleting files and directories
- [ ] Watching files (fs.watch, chokidar)
- [ ] Path module
- [ ] Async vs Sync file operations
- [ ] fs.promises API

### 📋 Interview Questions
1. How do you read a file in Node.js?
2. What is the difference between `readFile` and `readFileSync`?
3. What is `createReadStream`? When should you use it?
4. How do you write to a file in Node.js?
5. How do you check if a file exists?
6. How do you delete a file or directory?
7. What is the `path` module? What are `path.join()` and `path.resolve()`?
8. What is `__dirname` and `__filename`?
9. What is the `fs.promises` API?
10. How do you watch for file changes?

---

## 4.23 Events & EventEmitter

### ✅ Important Topics
- [ ] EventEmitter class
- [ ] Emitting events
- [ ] Listening for events (on, once, addListener)
- [ ] Removing listeners
- [ ] Custom EventEmitter
- [ ] Event-driven architecture
- [ ] Error event handling
- [ ] Max listeners warning

### 📋 Interview Questions
1. What is the EventEmitter class in Node.js?
2. How do you create a custom EventEmitter?
3. What is the difference between `on()` and `once()`?
4. How do you remove an event listener?
5. What happens if you emit an 'error' event with no listener?
6. What is the default maximum number of listeners?
7. How is EventEmitter used internally in Node.js? (Streams, HTTP server)
8. What is event-driven architecture?
9. How do you pass data with events?
10. What is the difference between `addListener` and `on`?

### 💻 Coding Questions
11. Create a custom EventEmitter class from scratch.
12. Implement a pub/sub system using EventEmitter.
13. Create a file watcher using EventEmitter.

---

## 4.24 Child Processes

### ✅ Important Topics
- [ ] exec()
- [ ] execFile()
- [ ] spawn()
- [ ] fork()
- [ ] IPC (Inter-Process Communication)
- [ ] Child process vs Worker Thread

### 📋 Interview Questions
1. What are child processes in Node.js?
2. What is the difference between `exec()`, `execFile()`, `spawn()`, and `fork()`?
3. When would you use `spawn()` over `exec()`?
4. What is `fork()`? How is it different from `spawn()`?
5. How do parent and child processes communicate?
6. What is IPC channel?
7. What is the difference between child processes and worker threads?
8. When would you use a child process?

---

### 🎯 What Interviewer Expects (Node.js)
- [ ] Understanding of Event Loop phases and execution order
- [ ] Knowledge of middleware pattern and implementation
- [ ] Understanding of authentication (JWT, sessions, OAuth)
- [ ] Ability to design RESTful APIs
- [ ] Knowledge of error handling patterns
- [ ] Understanding of scalability and performance optimization
- [ ] Awareness of security best practices
- [ ] Understanding of streams and when to use them
- [ ] Knowledge of Node.js internals (libuv, V8, Event Loop)
- [ ] Practical experience with Express.js

### ❌ Common Mistakes (Node.js)
- [ ] Blocking the Event Loop with synchronous operations
- [ ] Not handling async errors properly (missing try/catch or .catch())
- [ ] Storing passwords in plain text
- [ ] Not validating user input
- [ ] Sending stack traces in production error responses
- [ ] Not using environment variables for secrets
- [ ] Not implementing rate limiting
- [ ] Using `var` instead of `const`/`let`
- [ ] Not closing database connections properly
- [ ] Ignoring `unhandledRejection` and `uncaughtException`
- [ ] Not using proper logging (relying on console.log in production)
- [ ] Calling `next()` after sending a response
- [ ] Not setting security headers
- [ ] Memory leaks from unclosed event listeners

### 🔥 Must Know Concepts (Node.js)
- [ ] Event Loop phases and execution order
- [ ] process.nextTick vs setImmediate vs setTimeout
- [ ] Middleware chain execution
- [ ] JWT authentication flow (sign, verify, refresh)
- [ ] Express error handling (global error handler, async error wrapper)
- [ ] MVC folder structure for Express
- [ ] Streams for large data processing
- [ ] Cluster module for multi-core utilization
- [ ] Security best practices (Helmet, CORS, rate limiting, input validation)
- [ ] REST API design principles
- [ ] PM2 for production deployment
- [ ] Environment variables and configuration management

---

> **📌 SECTION 4 COMPLETE — Node.js**
>
> Say **"Continue"** to generate **Section 5: MongoDB** and **Section 6: SQL**

---
