# ═══════════════════════════════════════════════════════
# SECTION 13: REST API (COMPLETE)
# ═══════════════════════════════════════════════════════

---

## 13.1 REST Architecture Fundamentals

### ✅ Important Topics
- [ ] What is an API?
- [ ] What is REST (Representational State Transfer)?
- [ ] 6 Guiding Principles of REST
- [ ] REST vs SOAP
- [ ] REST vs GraphQL
- [ ] Resources and URIs (Uniform Resource Identifiers)
- [ ] Naming Conventions for Endpoints

### 📋 Interview Questions
1. What is an API? What is a RESTful API?
2. What are the six architectural constraints of REST? (Client-Server, Stateless, Cacheable, Uniform Interface, Layered System, Code on Demand).
3. What does it mean for a REST API to be "Stateless"? Why is this important for scalability?
4. How is REST different from SOAP?
5. How is REST different from GraphQL? When would you choose one over the other?
6. What is a URI? What is the difference between a URI and a URL?
7. What are the best practices for naming REST API endpoints? (e.g., Use nouns not verbs, use plurals).
8. Is `/getUsers` a good REST API endpoint name? Why or why not? What is the alternative?

---

## 13.2 HTTP Methods & Idempotency

### ✅ Important Topics
- [ ] GET, POST, PUT, PATCH, DELETE, OPTIONS
- [ ] Safe Methods
- [ ] Idempotency
- [ ] PUT vs PATCH
- [ ] POST vs PUT

### 📋 Interview Questions
1. Explain the primary HTTP methods used in REST APIs and their CRUD mappings.
2. What is a "Safe" HTTP method? Which methods are considered safe?
3. What is "Idempotency" in REST? Why is it a critical concept?
4. Which HTTP methods are idempotent? Which are not?
5. Is the `GET` method idempotent? Is `DELETE` idempotent?
6. What is the exact difference between `PUT` and `PATCH`?
7. What is the difference between `POST` and `PUT`? When would you use each to create a resource?
8. What is the `OPTIONS` method used for? (CORS preflight requests).

---

## 13.3 HTTP Status Codes

### ✅ Important Topics
- [ ] 1xx (Informational)
- [ ] 2xx (Success)
- [ ] 3xx (Redirection)
- [ ] 4xx (Client Errors)
- [ ] 5xx (Server Errors)
- [ ] Specific codes: 200, 201, 204, 301, 302, 400, 401, 403, 404, 405, 409, 429, 500, 502, 503

### 📋 Interview Questions
1. Explain the five classes of HTTP status codes.
2. What is the difference between `200 OK` and `201 Created`? When should you use `201`?
3. What does a `204 No Content` status code mean? Which HTTP method commonly returns this?
4. What is the difference between `301 Moved Permanently` and `302 Found`?
5. What is the exact difference between `401 Unauthorized` and `403 Forbidden`?
6. What does `400 Bad Request` mean? When should a server return it?
7. What is a `404 Not Found` error? What is a `405 Method Not Allowed` error?
8. When handling a registration API, if the email already exists, what status code should you return? (`409 Conflict`).
9. What status code is used for Rate Limiting? (`429 Too Many Requests`).
10. What is the difference between a `500 Internal Server Error` and a `502 Bad Gateway`?

---

## 13.4 HTTP Headers

### ✅ Important Topics
- [ ] Request Headers vs Response Headers
- [ ] Content-Type vs Accept
- [ ] Authorization Header
- [ ] Cache-Control
- [ ] ETag
- [ ] User-Agent

### 📋 Interview Questions
1. What are HTTP Headers? Why are they used?
2. What is the difference between the `Content-Type` header and the `Accept` header?
3. How do you pass a JWT token in an HTTP request? (In the `Authorization` header as a Bearer token).
4. What is the `Cache-Control` header?
5. What is an `ETag` (Entity Tag)? How does it help with caching and conditional requests?
6. What information does the `User-Agent` header provide?

---

## 13.5 API Design: Pagination, Filtering, Sorting & Versioning

### ✅ Important Topics
- [ ] Offset-based vs Cursor-based Pagination
- [ ] Query Parameters for Filtering and Sorting
- [ ] API Versioning Strategies (URI, Query, Header)

### 📋 Interview Questions
1. If you have an endpoint `/users` that returns 10 million records, how do you handle it? (Pagination).
2. What is Offset-based pagination? What are its drawbacks for large datasets? (e.g., `?limit=10&offset=100`).
3. What is Cursor-based pagination? Why is it more performant than offset-based?
4. How do you implement Filtering and Sorting in a REST API? Where should these parameters go? (Query string).
5. Why is API Versioning important?
6. What are the different ways to version a REST API? (URI versioning like `/v1/users`, Query parameter, Header versioning). Which is the most common?

---

## 13.6 REST API Security

### ✅ Important Topics
- [ ] HTTPS / TLS
- [ ] Authentication vs Authorization
- [ ] Input Validation & Sanitization
- [ ] Rate Limiting
- [ ] CORS (Cross-Origin Resource Sharing)

### 📋 Interview Questions
1. How do you secure a REST API?
2. Why must REST APIs be served over HTTPS?
3. What is CORS? How does the browser enforce it?
4. How do you protect your API against SQL/NoSQL Injection? (Input validation, parameterized queries/ORMs).
5. How do you protect against brute-force attacks on a login endpoint? (Rate limiting, account lockout).
6. Should you ever send sensitive data (like passwords) in a GET request query string? Why not? (They get logged in browser history and server access logs).

### 🎯 Scenario Based Questions
7. **Scenario:** You are building a blog API. Design the RESTful endpoints for viewing all posts, viewing a single post, creating a post, updating a post's title, and deleting a post.
8. **Scenario:** A user is trying to delete a resource they do not own. What HTTP status code should your API return? (`403 Forbidden`).
9. **Scenario:** Your API is suddenly receiving 100x normal traffic from a single IP address, causing the database to crash. What architecture component is missing? (Rate Limiter).

---

### 🎯 What Interviewer Expects (REST API)
- [ ] Flawless knowledge of HTTP Methods (especially PUT vs PATCH) and Idempotency.
- [ ] Knowing exactly which Status Code to return in specific scenarios.
- [ ] Ability to design clean, noun-based, pluralized API endpoints.
- [ ] Understanding of how to implement pagination for performance.

### ❌ Common Mistakes (REST API)
- [ ] Using verbs in endpoint URIs (e.g., `/create-user` instead of `POST /users`).
- [ ] Returning `200 OK` for every response, even errors, and placing the error code inside the JSON payload (anti-pattern).
- [ ] Confusing `401 Unauthorized` (not logged in) with `403 Forbidden` (logged in but lacks permission).

---

> **📌 SECTION 13 COMPLETE — REST API**
>
> Say **"Continue"** to generate **Section 14: Authentication**

---
