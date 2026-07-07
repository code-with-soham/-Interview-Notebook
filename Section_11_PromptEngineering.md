# ═══════════════════════════════════════════════════════
# SECTION 11: PROMPT ENGINEERING & AI FUNDAMENTALS
# ═══════════════════════════════════════════════════════

---

## 11.1 Artificial Intelligence Basics

### ✅ Important Topics
- [ ] What is AI, ML, and DL? (Differences)
- [ ] What is Generative AI?
- [ ] Natural Language Processing (NLP)
- [ ] Foundation Models vs Fine-tuned Models
- [ ] Tokens and Tokenization
- [ ] Context Window
- [ ] Hallucinations

### 📋 Interview Questions
1. How would you explain Artificial Intelligence, Machine Learning, and Deep Learning to a non-technical person?
2. What makes "Generative AI" different from traditional Machine Learning?
3. What is Natural Language Processing (NLP)?
4. What is a Token in the context of LLMs? Is one token equal to one word?
5. What is a Context Window? Why is it a limiting factor in LLMs?
6. What are AI "Hallucinations"? Why do they happen?
7. How can you mitigate or reduce AI hallucinations in a production application?
8. What is the difference between a Foundation Model (like GPT-4 or Gemini Pro) and a Domain-Specific Model?

---

## 11.2 Prompt Engineering Principles

### ✅ Important Topics
- [ ] What is Prompt Engineering?
- [ ] Anatomy of a good prompt (Role, Task, Context, Format)
- [ ] System Prompts vs User Prompts
- [ ] Temperature, Top-P, and Top-K (Generation parameters)
- [ ] Zero-shot Prompting
- [ ] One-shot and Few-shot Prompting
- [ ] Chain of Thought (CoT) Prompting
- [ ] Tree of Thoughts (ToT)

### 📋 Interview Questions
1. What is Prompt Engineering? Why is it considered a necessary skill for modern developers?
2. What are the key components of a highly effective prompt?
3. What is the difference between a "System Instruction/Prompt" and a "User Prompt"?
4. What does the "Temperature" parameter do in an LLM API? When would you use a Temperature of 0.0 vs 0.9?
5. What are Top-P and Top-K sampling methods?
6. What is Zero-shot prompting?
7. How does Few-shot prompting improve model performance compared to Zero-shot?
8. What is "Chain of Thought" (CoT) prompting? ("Let's think step by step")
9. Why does asking an LLM to explain its reasoning *before* giving the final answer produce better results?
10. What is "Tree of Thoughts" (ToT) prompting?

---

## 11.3 Advanced Prompting Techniques

### ✅ Important Topics
- [ ] Retrieval-Augmented Generation (RAG) concepts
- [ ] Prompt Chaining / Sequential Prompting
- [ ] Self-Consistency
- [ ] ReAct (Reasoning and Acting) Framework
- [ ] Prompt Injection & Security

### 📋 Interview Questions
1. What is Prompt Chaining? How is it different from passing one giant prompt?
2. What is the ReAct (Reason+Act) prompting framework? How does it enable AI Agents?
3. What is Self-Consistency in prompting?
4. What is Prompt Injection? Give an example of how a malicious user might exploit an AI chatbot.
5. How do you protect your LLM application against Prompt Injection attacks?
6. What is Jailbreaking in the context of LLMs?
7. What are the limitations of Prompt Engineering? When should you stop tweaking prompts and start fine-tuning?

---

## 11.4 Practical AI Integration Scenarios

### 🎯 Scenario Based Questions
1. **Scenario:** You are building an AI customer support bot. It keeps giving confident but incorrect answers about your company's refund policy. How do you fix this using prompt engineering?
2. **Scenario:** You need the LLM to output strict JSON data so your backend Node.js server can parse it. However, the model keeps adding text like "Here is your JSON:" before the output. How do you fix this via the prompt or API parameters?
3. **Scenario:** You want an LLM to summarize a 100-page PDF document, but it exceeds the model's Context Window. How do you approach this problem?
4. **Scenario:** Users are submitting queries to your AI app, but the responses are too generic. How do you use the "Role" or "Persona" technique to improve the output?

---

### 🎯 What Interviewer Expects (Prompt Engineering)
- [ ] Understanding that prompting is not just "talking to AI", but structuring deterministic inputs for probabilistic models.
- [ ] Clear knowledge of Temperature and formatting.
- [ ] Deep understanding of Zero-shot, Few-shot, and Chain of Thought.
- [ ] Awareness of AI security risks (Prompt Injection).
- [ ] Ability to force an LLM into predictable formats (JSON, XML).

### ❌ Common Mistakes (Prompt Engineering)
- [ ] Thinking Prompt Engineering is just writing polite sentences.
- [ ] Not understanding what a Token or Context Window is.
- [ ] Confusing Temperature with model accuracy (Low temp doesn't mean correct, it means deterministic).
- [ ] Trying to solve lack of knowledge with prompt engineering instead of RAG/Fine-tuning.

---

> **📌 SECTION 11 COMPLETE — Prompt Engineering & AI**
