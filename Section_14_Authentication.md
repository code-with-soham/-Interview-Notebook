# ═══════════════════════════════════════════════════════
# SECTION 14: AUTHENTICATION & SECURITY (COMPLETE)
# ═══════════════════════════════════════════════════════

---

## 14.1 Authentication vs Authorization

### ✅ Important Topics
- [ ] Authentication (AuthN)
- [ ] Authorization (AuthZ)
- [ ] Identity Verification vs Permission Checking

### 📋 Interview Questions
1. What is the fundamental difference between Authentication and Authorization?
2. Can Authorization happen without Authentication?
3. Give a real-world analogy for Authentication vs Authorization.

---

## 14.2 Session-Based vs Token-Based Authentication

### ✅ Important Topics
- [ ] Session-Based Authentication (Stateful)
- [ ] Token-Based Authentication (Stateless)
- [ ] Cookies vs Local Storage
- [ ] Scalability implications

### 📋 Interview Questions
1. How does Session-based authentication work?
2. Where is session data typically stored on the server? (Memory, Database, Redis).
3. Why is Session-based authentication considered "Stateful"?
4. What are the challenges of Session-based authentication in a horizontally scaled system (multiple servers)?
5. How does Token-based authentication solve the scalability issue of sessions?
6. Is Token-based authentication stateful or stateless?

---

## 14.3 JSON Web Tokens (JWT)

### ✅ Important Topics
- [ ] JWT Structure (Header, Payload, Signature)
- [ ] Base64Url Encoding
- [ ] JWT Signing and Verification
- [ ] JWT Claims (`sub`, `exp`, `iat`)
- [ ] Security concerns with JWT

### 📋 Interview Questions
1. What does JWT stand for? What are its three main parts?
2. What is contained in the Payload of a JWT? What kind of data should you NEVER put in the payload?
3. How is the Signature of a JWT generated?
4. Are JWTs encrypted by default? Can anyone read the payload?
5. If anyone can decode a JWT, how does the server know it hasn't been tampered with? (The Signature).
6. How do you invalidate or revoke a JWT before it expires? (Blacklisting, changing the secret).
7. Why is storing a JWT in Local Storage considered a bad practice? (Vulnerable to XSS).
8. What is the most secure way to store a JWT on the client side? (HttpOnly, Secure, SameSite Cookie).

---

## 14.4 Access Tokens & Refresh Tokens

### ✅ Important Topics
- [ ] Access Token lifecycle
- [ ] Refresh Token lifecycle
- [ ] Token Rotation
- [ ] Security tradeoffs

### 📋 Interview Questions
1. What is an Access Token? What is its typical lifespan?
2. What is a Refresh Token? Why do we need it?
3. Explain the flow of using an Access Token and a Refresh Token when the Access Token expires.
4. Where should you store the Refresh Token? (HttpOnly Cookie, Database for revocation).
5. What happens if a Refresh Token is stolen? How do you mitigate this? (Refresh Token Rotation / Family of tokens).

---

## 14.5 OAuth 2.0 & Single Sign-On (SSO)

### ✅ Important Topics
- [ ] OAuth 2.0 Roles (Resource Owner, Client, Authorization Server, Resource Server)
- [ ] Authorization Code Flow
- [ ] Single Sign-On (SSO)
- [ ] OpenID Connect (OIDC) vs OAuth

### 📋 Interview Questions
1. What is OAuth 2.0? Is it an authentication protocol or an authorization protocol? (Authorization).
2. What are the four main roles in OAuth 2.0?
3. Explain the standard OAuth 2.0 Authorization Code Flow. (e.g., "Login with Google").
4. What is Single Sign-On (SSO)? How does it benefit user experience and security?
5. What is the difference between OAuth 2.0 and OpenID Connect (OIDC)?

---

## 14.6 Web Security Vulnerabilities (XSS, CSRF, CORS)

### ✅ Important Topics
- [ ] XSS (Cross-Site Scripting)
- [ ] CSRF (Cross-Site Request Forgery)
- [ ] CORS (Cross-Origin Resource Sharing)
- [ ] Same-Origin Policy (SOP)
- [ ] Mitigation strategies

### 📋 Interview Questions
1. What is XSS (Cross-Site Scripting)? Explain the difference between Stored and Reflected XSS.
2. How does an attacker exploit an XSS vulnerability to steal a JWT stored in Local Storage?
3. How do you prevent XSS attacks? (Sanitize input, escape output, use HttpOnly cookies).
4. What is CSRF (Cross-Site Request Forgery)? How does it work?
5. If you store your JWT in an HttpOnly cookie (which prevents XSS), what new vulnerability does this introduce? (CSRF).
6. How do you prevent CSRF attacks? (Anti-CSRF tokens, SameSite cookie attribute).
7. What is the Same-Origin Policy (SOP) in browsers?
8. What is CORS? Why does the browser block requests from different origins?
9. Explain the CORS Preflight request (`OPTIONS`). What headers does the server need to return to allow the request? (`Access-Control-Allow-Origin`).

### 🎯 Scenario Based Questions
10. **Scenario:** A user logs out of your React application, but their JWT is still valid for 30 minutes. How do you ensure that token cannot be used again?
11. **Scenario:** You are building an API that will be accessed by a mobile app and a web app. Should you use cookies or Bearer tokens in the Authorization header?
12. **Scenario:** Your web application allows users to submit comments with HTML formatting. How do you ensure malicious scripts aren't executed when other users view the comment?

---

### 🎯 What Interviewer Expects (Authentication)
- [ ] Perfect understanding of the JWT structure and its stateless nature.
- [ ] Knowing exactly *where* to store tokens securely (HttpOnly Cookies vs Local Storage) and the tradeoffs (CSRF vs XSS).
- [ ] Understanding the Access + Refresh token flow.
- [ ] Solid grasp of CORS, as it is the most common issue Full Stack developers face during integration.

### ❌ Common Mistakes (Authentication)
- [ ] Confusing Authentication with Authorization.
- [ ] Thinking JWTs are encrypted and therefore safe to hold sensitive data like passwords or PII.
- [ ] Believing you can easily "destroy" a stateless JWT on the server side just by logging out the user on the client side.

---

> **📌 SECTION 14 COMPLETE — Authentication**
>
> Say **"Continue"** to generate **Section 15: AI (LLM, Prompt Engineering, RAG, Gemini)**

---
