# ═══════════════════════════════════════════════════════
# SECTION 12: DOCKER & CONTAINERIZATION (COMPLETE)
# ═══════════════════════════════════════════════════════

---

## 12.1 Docker Fundamentals

### ✅ Important Topics
- [ ] What is Docker?
- [ ] Virtual Machines vs Containers
- [ ] Docker Architecture (Client, Host, Registry)
- [ ] Docker Daemon
- [ ] Docker Images vs Docker Containers
- [ ] Docker Hub

### 📋 Interview Questions
1. What is Docker? What problem does it solve in software development?
2. Explain the fundamental difference between a Docker Container and a Virtual Machine (VM).
3. What is the Docker Daemon? What is its role?
4. What is a Docker Image? Is it mutable or immutable?
5. What is a Docker Container? How does it relate to an Image?
6. What is the difference between an Image Registry (like Docker Hub) and a Repository?
7. Explain the lifecycle of a Docker Container.

---

## 12.2 Dockerfile & Image Creation

### ✅ Important Topics
- [ ] What is a Dockerfile?
- [ ] Common instructions (`FROM`, `RUN`, `CMD`, `ENTRYPOINT`, `COPY`, `ADD`, `ENV`, `EXPOSE`, `WORKDIR`)
- [ ] `.dockerignore` file
- [ ] Building images (`docker build`)

### 📋 Interview Questions
1. What is a Dockerfile?
2. What is the purpose of the `FROM` instruction? Can a Dockerfile have multiple `FROM` instructions? (Hint: Multi-stage builds).
3. What is the exact difference between `RUN`, `CMD`, and `ENTRYPOINT`?
4. What happens if you define multiple `CMD` instructions in a single Dockerfile?
5. What is the difference between `COPY` and `ADD`? Which one is preferred and why?
6. What does the `EXPOSE` instruction do? Does it actually publish the port to the host machine?
7. What is a `.dockerignore` file? Why is it crucial, especially for Node.js applications? (e.g., ignoring `node_modules`).

---

## 12.3 Docker Layers & Optimization

### ✅ Important Topics
- [ ] Docker Image Layers
- [ ] Layer Caching
- [ ] Multi-stage Builds
- [ ] Alpine Linux Images
- [ ] Minimizing Image Size

### 📋 Interview Questions
1. Explain how Docker Image Layers work.
2. How does Docker utilize caching during the `docker build` process?
3. In a Node.js Dockerfile, why is it recommended to `COPY package.json` and run `npm install` *before* copying the rest of the application code?
4. What are Multi-stage builds? How do they help in reducing the final image size?
5. What is an Alpine image? Why is it popular in the Docker ecosystem?
6. How do you reduce the size of a Docker image? (Multi-stage builds, minimizing layers, using smaller base images, `.dockerignore`).

---

## 12.4 Docker Storage & Volumes

### ✅ Important Topics
- [ ] Ephemeral Storage vs Persistent Storage
- [ ] Bind Mounts
- [ ] Docker Volumes
- [ ] tmpfs Mounts

### 📋 Interview Questions
1. Are Docker containers ephemeral? What happens to the data inside a container when it is deleted?
2. How do you achieve data persistence in Docker?
3. What is a Docker Volume? How is it different from a Bind Mount?
4. When would you use a Bind Mount instead of a Volume? (e.g., Local development with hot-reloading).
5. Where are Docker Volumes stored on the host machine?
6. How do you share data between multiple Docker containers?

---

## 12.5 Docker Networking

### ✅ Important Topics
- [ ] Default networks (bridge, host, none)
- [ ] User-defined bridge networks
- [ ] Port mapping/publishing (`-p`)
- [ ] DNS resolution between containers

### 📋 Interview Questions
1. What are the default network drivers available in Docker?
2. What is the `bridge` network? How does it isolate containers?
3. What is the `host` network? What are its security implications?
4. How do you expose a container's port to the outside world? (Explain `docker run -p 8080:80`).
5. If two containers are on the same custom bridge network, how do they communicate with each other? (By container name via internal DNS).

---

## 12.6 Docker Compose

### ✅ Important Topics
- [ ] What is Docker Compose?
- [ ] `docker-compose.yml` syntax
- [ ] Services, Networks, Volumes in Compose
- [ ] Commands (`up`, `down`, `build`, `ps`)

### 📋 Interview Questions
1. What is Docker Compose? When and why would you use it instead of the standard Docker CLI?
2. In a `docker-compose.yml` file, what is a `service`?
3. How do you ensure that your backend service starts only *after* your database service has started in Docker Compose? (Hint: `depends_on`).
4. What is the difference between `docker-compose up` and `docker-compose up --build`?
5. How do you stop and remove all containers, networks, and volumes defined in a Compose file? (`docker-compose down -v`).

### 🎯 Scenario Based Questions
6. **Scenario:** You are dockerizing a MERN stack application. Walk me through how you would set up your `docker-compose.yml` file. How many services would you have? How do they communicate?
7. **Scenario:** You notice your Docker build is taking 10 minutes every time you change a single line of CSS. How do you fix this layer caching issue?
8. **Scenario:** Your Node.js API container cannot connect to your MongoDB container. Both are running via `docker run`. What is the most likely networking issue?

---

### 🎯 What Interviewer Expects (Docker)
- [ ] Clear understanding that Containers share the host OS kernel, unlike VMs.
- [ ] Ability to write an optimized Dockerfile (Layer caching, Multi-stage builds).
- [ ] Understanding of how data persists using Volumes.
- [ ] Ability to orchestrate a multi-container local dev environment using Docker Compose.

### ❌ Common Mistakes (Docker)
- [ ] Thinking a container is a full virtual machine.
- [ ] Putting database credentials or API keys directly in the Dockerfile instead of passing them as Environment Variables.
- [ ] Copying `node_modules` into the image instead of installing them inside the build process.
- [ ] Running processes as the `root` user inside the container in production (security risk).

---

> **📌 SECTION 12 COMPLETE — Docker**
>
> Say **"Continue"** to generate **Section 13: REST API**

---
