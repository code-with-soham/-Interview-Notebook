# ═══════════════════════════════════════════════════════
# SECTION 14: DOCKER & DEPLOYMENT
# ═══════════════════════════════════════════════════════

---

## 14.1 Docker Fundamentals

### ✅ Important Topics
- [ ] What is Docker?
- [ ] Virtual Machines vs Containers
- [ ] Docker Image vs Docker Container
- [ ] Dockerfile
- [ ] Docker Hub / Container Registries
- [ ] Docker Volumes
- [ ] Docker Networks

### 📋 Interview Questions
1. What is Docker? Why is it so widely used in modern software development?
2. Explain the difference between a Virtual Machine (VM) and a Docker Container.
3. What is a Docker Image?
4. What is a Docker Container? How is it related to an Image?
5. What is a Dockerfile?
6. What is the difference between the `RUN`, `CMD`, and `ENTRYPOINT` instructions in a Dockerfile?
7. What is the difference between `COPY` and `ADD` in a Dockerfile?
8. Why should you try to minimize the number of layers in a Docker Image?
9. What are Docker Volumes? Why do we need them? (Data persistence).
10. What is a Docker Network? How do containers talk to each other?

---

## 14.2 Docker Compose

### ✅ Important Topics
- [ ] What is Docker Compose?
- [ ] docker-compose.yml structure
- [ ] Multi-container applications

### 📋 Interview Questions
1. What is Docker Compose? When would you use it instead of just running `docker run` commands?
2. How do you define services, networks, and volumes in a `docker-compose.yml` file?
3. In a Docker Compose setup with a Node.js backend and a MongoDB database, how does the Node.js app connect to the database? (Using the service name as the hostname).
4. What is the difference between `docker-compose up` and `docker-compose up -d`?

---

## 14.3 CI/CD (Continuous Integration / Continuous Deployment)

### ✅ Important Topics
- [ ] What is CI/CD?
- [ ] Continuous Integration vs Continuous Delivery vs Continuous Deployment
- [ ] GitHub Actions basics
- [ ] Build pipelines

### 📋 Interview Questions
1. What does CI/CD stand for? Explain the concepts.
2. What is the difference between Continuous Delivery and Continuous Deployment?
3. What are GitHub Actions?
4. Describe a standard CI/CD pipeline for a MERN stack application. (Lint -> Test -> Build Image -> Push to Registry -> Deploy to Server).
5. Why is automated testing a crucial part of CI/CD?

---

## 14.4 Cloud & Deployment Basics (Fresher Level)

### ✅ Important Topics
- [ ] IaaS vs PaaS vs SaaS
- [ ] AWS EC2, S3 basics
- [ ] Vercel, Heroku, Netlify, Render
- [ ] Nginx (Reverse Proxy)
- [ ] PM2 (Process Manager)

### 📋 Interview Questions
1. What is the difference between IaaS (Infrastructure as a Service), PaaS (Platform as a Service), and SaaS (Software as a Service)?
2. If you deploy a React frontend to Vercel and a Node backend to Render, what type of cloud services are you using? (PaaS).
3. What is AWS EC2?
4. What is AWS S3 used for?
5. What is a Reverse Proxy? Why would you use Nginx in front of a Node.js server?
6. What is PM2? Why do you need it to run a Node.js app on a server? (Process management, auto-restart on crash).
7. How do you map a custom domain name to your deployed application? (DNS A Records / CNAME).

---

### 🎯 What Interviewer Expects (Docker & Deployment)
- [ ] Understanding that Docker solves the "It works on my machine" problem.
- [ ] Knowing how to write a basic `Dockerfile` for a Node.js or React app.
- [ ] Understanding data persistence (Volumes).
- [ ] Knowing what CI/CD is conceptually.
- [ ] Knowing how a full-stack app is actually hosted in the real world (Frontend on CDN/Vercel, Backend on VM/Render, DB on Atlas).

### ❌ Common Mistakes (Docker & Deployment)
- [ ] Thinking a Docker container is a full virtual machine with its own OS kernel.
- [ ] Hardcoding API keys or database passwords into a Dockerfile instead of using Environment Variables (`ENV` / `.env`).
- [ ] Not understanding that containers are ephemeral (if you delete the container without a volume, the data is gone).

---

> **📌 SECTION 14 COMPLETE — Docker & Deployment**
>
> Say **"Continue"** to generate **Section 15: Behavioral & HR Questions** (The final core section).

---
