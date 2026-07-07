# ═══════════════════════════════════════════════════════
# SECTION 7: SYSTEM DESIGN BASICS (COMPLETE)
# ═══════════════════════════════════════════════════════

---

## 7.1 Architecture Fundamentals

### ✅ Important Topics
- [ ] Client-Server Architecture
- [ ] Monolith vs Microservices
- [ ] API Gateway
- [ ] Reverse Proxy
- [ ] Load Balancer

### 📋 Interview Questions
1. What is the difference between a Monolithic and Microservices architecture?
2. What are the advantages and disadvantages of Microservices?
3. What is an API Gateway? Why is it used in Microservices?
4. What is a Reverse Proxy? How is it different from a Forward Proxy?
5. What is a Load Balancer? At which OSI layers can a Load Balancer operate?
6. What are common Load Balancing algorithms? (Round Robin, Least Connections, IP Hash)

---

## 7.2 Scalability & Performance

### ✅ Important Topics
- [ ] Scalability Concepts
- [ ] Horizontal Scaling (Scale-out)
- [ ] Vertical Scaling (Scale-up)
- [ ] Caching
- [ ] Redis
- [ ] CDN (Content Delivery Network)

### 📋 Interview Questions
1. What is the difference between Horizontal and Vertical scaling?
2. When would you choose Vertical scaling over Horizontal scaling?
3. What are the challenges of Horizontal scaling?
4. What is caching? At what layers can caching be implemented in a system?
5. What is Redis? How does it differ from a relational database?
6. What are common cache eviction policies? (LRU, LFU, FIFO)
7. What is cache penetration, cache breakdown, and cache avalanche?
8. What is a CDN? How does it improve application performance?
9. What type of content is best suited for a CDN?

---

## 7.3 Communication Protocols

### ✅ Important Topics
- [ ] Polling
- [ ] Long Polling
- [ ] WebSocket
- [ ] Server-Sent Events (SSE)
- [ ] Message Queues

### 📋 Interview Questions
1. What is short polling? Why is it generally inefficient?
2. What is long polling? How does it improve upon short polling?
3. What is a WebSocket? How does the handshake process work?
4. When would you use WebSockets over HTTP?
5. What are Server-Sent Events (SSE)? How are they different from WebSockets?
6. Compare Polling, Long Polling, WebSockets, and SSE. Which one would you choose for a real-time chat app? Which for a stock ticker?
7. What is a Message Queue? (e.g., RabbitMQ, Kafka)
8. What is the Publisher/Subscriber (Pub/Sub) pattern?
9. Why use message queues in a distributed system? (Decoupling, asynchronous processing, peak load buffering).

---

## 7.4 Security & Rate Limiting

### ✅ Important Topics
- [ ] Authentication
- [ ] Authorization
- [ ] Rate Limiting

### 📋 Interview Questions
1. What is the difference between Authentication and Authorization?
2. How do you implement stateless authentication in a distributed system?
3. What is Rate Limiting? Why is it crucial for APIs?
4. Explain the Token Bucket algorithm for rate limiting.
5. Explain the Leaky Bucket algorithm.
6. Explain the Sliding Window algorithm.
7. Where should Rate Limiting be implemented in your architecture? (API Gateway, App Server, Load Balancer?)

### 🎯 Scenario Based Questions
8. Your e-commerce website is crashing during a flash sale. What system design components would you add to handle the spike in traffic?
9. You need to build a real-time collaborative document editor (like Google Docs). What communication protocol would you use and why?
10. A user's request takes 5 seconds to process because it involves generating a PDF. How would you redesign this using message queues?

---

### 🎯 What Interviewer Expects (System Design)
- [ ] Clear understanding of when to use Monolith vs Microservices.
- [ ] Ability to identify where caching is needed.
- [ ] Understanding the tradeoffs between WebSockets, SSE, and Polling.
- [ ] Basic knowledge of how to prevent API abuse (Rate Limiting).

### ❌ Common Mistakes (System Design)
- [ ] Suggesting Microservices for every single problem (over-engineering).
- [ ] Confusing Authentication with Authorization.
- [ ] Not knowing the difference between an API Gateway and a Load Balancer.

---

> **📌 SECTION 7 COMPLETE — System Design Basics**
>
> Say **"Continue"** to generate **Section 8: Operating System**

---
