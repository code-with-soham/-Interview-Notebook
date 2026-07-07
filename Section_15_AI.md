# ═══════════════════════════════════════════════════════
# SECTION 15: ARTIFICIAL INTELLIGENCE & LLMS (COMPLETE)
# ═══════════════════════════════════════════════════════

---

## 15.1 Generative AI & LLM Fundamentals

### ✅ Important Topics
- [ ] What is an LLM (Large Language Model)?
- [ ] Transformer Architecture
- [ ] Self-Attention Mechanism
- [ ] Tokens and Tokenization
- [ ] Context Window
- [ ] Inference vs Training
- [ ] Latency vs Throughput (TTFT, TPS)
- [ ] Hallucination

### 📋 Interview Questions
1. What is a Large Language Model (LLM)?
2. What is the Transformer architecture? Why did it revolutionize NLP compared to RNNs and LSTMs?
3. Explain the "Self-Attention" mechanism in simple terms.
4. What is a Token? Is a token exactly equal to one word?
5. What is the Context Window of an LLM? Why does performance often degrade as the context window fills up?
6. What is the difference between Model Training, Fine-Tuning, and Inference?
7. In the context of LLM Inference, what do TTFT (Time To First Token) and TPS (Tokens Per Second) mean?
8. What is AI Hallucination? What causes a model to hallucinate?

---

## 15.2 Prompt Engineering & Model Parameters

### ✅ Important Topics
- [ ] Prompt Engineering Techniques (Zero-shot, Few-shot, Chain of Thought)
- [ ] Temperature
- [ ] Top-K and Top-P
- [ ] System vs User Prompts

### 📋 Interview Questions
1. What is Prompt Engineering? Why is it a deterministic approach to a probabilistic model?
2. Explain the `Temperature` parameter. What happens if you set it to 0.0 vs 1.0?
3. How do Top-K and Top-P sampling affect the model's output?
4. What is Zero-shot prompting vs Few-shot prompting?
5. What is "Chain of Thought" (CoT) prompting? Why does asking the model to "think step by step" improve accuracy on complex reasoning tasks?
6. What is the difference between a System Instruction and a User Prompt?

---

## 15.3 Embeddings & RAG (Retrieval-Augmented Generation)

### ✅ Important Topics
- [ ] Vector Embeddings
- [ ] Vector Databases (Pinecone, Chroma, MongoDB Atlas Vector Search)
- [ ] RAG Pipeline (Retrieval + Generation)
- [ ] Document Chunking Strategies
- [ ] Cosine Similarity

### 📋 Interview Questions
1. What is a Vector Embedding? How does it represent semantic meaning?
2. What is a Vector Database? How is it different from a standard relational database?
3. Explain the complete Retrieval-Augmented Generation (RAG) pipeline.
4. Why use RAG instead of just Fine-Tuning an LLM on your private data?
5. What is "Chunking" in the context of RAG? What happens if your chunks are too large or too small?
6. How does a Vector Database retrieve relevant documents? (Explain Cosine Similarity or Euclidean Distance).
7. If your RAG system is retrieving the right documents but the LLM is still giving the wrong answer, what part of the pipeline is failing?

---

## 15.4 AI Agents, Tool Calling & MCP

### ✅ Important Topics
- [ ] AI Agents vs Standard LLMs
- [ ] Function Calling / Tool Calling
- [ ] MCP (Model Context Protocol)

### 📋 Interview Questions
1. What defines an "AI Agent" compared to a standard chatbot? (Reasoning + Acting + Tool Use).
2. What is Function Calling (or Tool Calling) in APIs like Gemini or OpenAI?
3. How does Function Calling actually work under the hood? (The LLM doesn't execute the function, it returns a JSON object requesting the application to run it).
4. What is the Model Context Protocol (MCP)? (Standardizing how AI models interact with data sources and tools locally/remotely).

---

## 15.5 LLM Providers & Frameworks

### ✅ Important Topics
- [ ] Gemini, OpenAI, Anthropic
- [ ] Groq API (LPU vs GPU)
- [ ] Fine-tuning (LoRA, PEFT)

### 📋 Interview Questions
1. Compare the major LLM providers: OpenAI (GPT), Google (Gemini), and Anthropic (Claude). What are their respective strengths?
2. What is Groq? How does their LPU (Language Processing Unit) differ from traditional NVIDIA GPUs for inference?
3. When would you choose to use the Groq API over the Gemini API? (Latency vs Multimodal capabilities).
4. What is Fine-Tuning? Mention lightweight fine-tuning methods like LoRA.

---

## 15.6 AI Security & Guardrails

### ✅ Important Topics
- [ ] Prompt Injection
- [ ] Jailbreaking
- [ ] Input/Output Guardrails

### 📋 Interview Questions
1. What is Prompt Injection? Give an example of how an attacker might manipulate an AI application.
2. How do you prevent Prompt Injection?
3. What is Jailbreaking an LLM?
4. What are Guardrails in AI applications? (Validating inputs before they reach the model, and checking outputs before showing them to the user).

### 🎯 Scenario Based Questions
5. **Scenario:** You built a customer support bot using RAG, but it is taking 8 seconds to respond. How do you optimize the latency? (Streaming, Groq, caching, smaller embedding model).
6. **Scenario:** Your AI app needs to fetch live stock prices. How do you implement this? (Function Calling/Tool use).
7. **Scenario:** A user asks your RAG bot a question completely unrelated to your company, and it answers using its pre-trained knowledge. How do you restrict it to *only* answer from the retrieved context?

---

### 🎯 What Interviewer Expects (AI)
- [ ] Clear understanding that RAG does *not* alter model weights.
- [ ] Solid grasp of Embeddings and how Vector Databases retrieve similar text.
- [ ] Understanding of Function Calling as the core mechanism behind AI Agents.
- [ ] Knowledge of the tradeoff between Latency (Groq) and Reasoning/Context size (Gemini/Claude).

### ❌ Common Mistakes (AI)
- [ ] Confusing Fine-Tuning with RAG.
- [ ] Thinking that setting Temperature to 0 makes the model 100% accurate (it only makes it deterministic, it can still hallucinate).
- [ ] Thinking the LLM directly executes API calls in Function Calling (the application executes it based on the LLM's structured output).

---

> **📌 SECTION 15 COMPLETE — Artificial Intelligence**
>
> Say **"Continue"** to generate **Section 16: Machine Learning**

---
