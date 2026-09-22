# Oracle — AI Agent

> An intelligent AI agent that searches the web, reads pages, and reasons step by step to answer any question with real-time information.

![Python](https://img.shields.io/badge/Python-3.11-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-0.100+-green)
![Groq](https://img.shields.io/badge/LLM-Groq%20Llama%203.3%2070B-orange)
![License](https://img.shields.io/badge/License-MIT-purple)

---

## What is Oracle?

Oracle is an AI agent built on the **ReAct (Reason + Act)** architecture. Unlike a regular chatbot that only uses its training data, Oracle has real tools it can use to interact with the world — searching the web, reading webpages, performing calculations, and checking real-time data.

When you ask Oracle a question, it does not just guess. It thinks, searches, reads, and reasons step by step until it finds a reliable answer.

---

## Demo

```
You: What are the latest AI developments this week?

Oracle:
  🔍 Searched: "latest AI developments this week"
  🌐 Read: https://techcrunch.com/...
  🔍 Searched: "AI news June 2026"
  🌐 Read: https://venturebeat.com/...

  This week saw three major developments in AI:
  1. Google DeepMind announced...
  2. OpenAI released...
  3. Meta open-sourced...
```

---

## How it works

```
User asks a question
        ↓
Oracle sends question + available tools to Llama 3.3 70B
        ↓
LLM decides: use a tool or answer directly?
        ↓
If tool needed → YOUR CODE calls the tool
        ↓
Tool result sent back to LLM
        ↓
LLM reasons with the result
        ↓
Repeat until final answer is ready
        ↓
Answer returned to user
```

This loop is called the **ReAct loop** — the foundation of every AI agent.

---

