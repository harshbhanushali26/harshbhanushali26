
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:1e3a8a&height=200&section=header&text=Harsh%20Bhanushali&fontSize=40&fontColor=ffffff&animation=fadeIn&fontAlignY=35"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1000&color=38BDF8&center=true&vCenter=true&width=700&lines=Agentic+AI+Developer;Structure+First%2C+Then+Build;RAG+Pipelines+%7C+Multi-Agent+Systems;Open+to+AI+Engineer+Roles" />
</p>

<p align="center">
  <a href="https://harshbhanushali26.github.io" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-harshbhanushali26.github.io-0ea5e9?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  &nbsp;
  <a href="https://www.linkedin.com/in/harshbhanushali0709/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-harshbhanushali0709-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  &nbsp;
  <a href="https://mail.google.com/mail/?view=cm&to=harshbhanu0709@gmail.com" target="_blank">
    <img src="https://img.shields.io/badge/Gmail-harshbhanu0709-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
</p>

---

## About Me

> *"I've shipped enough broken AI projects to know — the architecture meeting you skip always becomes the bug you can't find."*

I'm an Agentic AI Developer from Gujarat, India. I build autonomous AI systems — RAG pipelines, multi-agent graphs, LLM-backed CLIs — and the one thing every project I've shipped has in common is that I planned the structure before writing a single line of code.

That habit didn't come from a course. It came from building things without it and feeling exactly what breaks and why. Now every project starts with a clear execution layer, defined state boundaries, and deliberate tradeoff decisions — before a file even gets created.

I work across the full AI engineering stack: from protocol-level MCP tool servers and LangGraph stateful graphs, to FastAPI backends and Streamlit interfaces that real users can actually interact with.

Currently building **Capsule** — a personal content manager with a Telegram bot frontend, FastAPI backend, Groq-powered processing, and hybrid SQLite + ChromaDB storage.

> 📍 Open to AI Engineer roles at AI-first startups — Mumbai, Pune, Bangalore, Hyderabad, or remote.

---

## 🏗️ Featured Projects

### 🔬 Multi-Agent Research Pipeline | [🔗 Repository](https://github.com/harshbhanushali26/research-pipeline)
*Autonomous CLI system executing structured, stateful research workflows across 6 specialized AI agents.*

- **Hierarchical Orchestration:** Designed a full supervisor-driven agent hierarchy — Supervisor → Search → Scrape → Summarize → Critique → Synthesize — with explicit state boundaries between each role to prevent context bleed across agents.
- **Quota-Aware Model Routing:** Built dynamic fallback logic using Groq (llama-3.3-70b) as primary and Gemini (gemini-2.0-flash) as fallback tier — agents switch models mid-pipeline without interrupting the workflow.
- **Human-in-the-Loop Checkpoints:** Engineered interactive review gates at critical pipeline stages with a clean Rich terminal UI, keeping a human in control without breaking the execution flow.
- **Stack:** Python, Groq, Gemini, DuckDuckGo, Rich CLI

---

### 🧠 hArI — RAG Document Intelligence | [🔗 Repository](https://github.com/harshbhanushali26/hArI)
*Production-deployed web app for grounded, hallucination-resistant document interrogation.*

- **Precision Retrieval:** Switched ChromaDB distance metric from L2 to cosine and enforced a strict `SCORE_THRESHOLD=0.35` — completely eliminated hallucinated source citations without touching the LLM layer.
- **Intent-Based Routing:** Built a local intent classifier that decides query path before hitting the vector store — Conversational → Vector RAG → LLM fallback — reducing unnecessary embedding lookups.
- **Clean Stream Output:** Wrote a custom `strip_thinking()` post-processor to scrub raw LLM reasoning tokens before they reach the UI, keeping responses clean without modifying the model behavior.
- **Stack:** Groq (llama-4-scout-17b), ChromaDB, SentenceTransformer (all-MiniLM-L6-v2), PyMuPDF, Streamlit, uv

---

### 🤖 AI Agent Engine | [🔗 Repository](https://github.com/harshbhanushali26/ai-agent-engine)
*A 4-layer autonomous agent pipeline built natively in Python — architected before a single file was created.*

- **Zero-LLM Routing Layer:** Designed a deterministic cache at the top of the pipeline that resolves ~80% of routine queries with 0 LLM API calls — speed and cost handled at the architecture level, not prompt level.
- **Sub-50ms Semantic Search:** Integrated ChromaDB + SentenceTransformer maintaining ~30ms semantic search latency as the second routing layer before any external API call is made.
- **Strict Execution Economics:** Planner → Validator → Executor pipeline with hard quota enforcement keeps per-session cost at ~$0.0005 — a constraint that was designed in, not optimized in later.
- **Stack:** Python 3.11+, Gemini API, ChromaDB, SentenceTransformer, DuckDuckGo, Open-Meteo

---
## 📦 Other Projects

| Project | What it does | Stack |
|--------|-------------|-------|
| [🔌 DevMind — MCP Server](https://github.com/harshbhanushali26/mcp-implementations) | Local Model Context Protocol tool server giving LLMs secure, HITL-gated access to the file system — read, write, execute Python snippets, format JSON, count tokens | Python, MCP SDK, tiktoken |
| [🗄️ LangGraph SQL Runner](https://github.com/harshbhanushali26) | Multi-question parallel SQL execution using LangGraph's Send API for dynamic fan-out across schema analysis and execution nodes, with inline HITL review before any query fires | LangGraph, Groq, SQLite, Pydantic |
| [💰 Finance Agent CLI](https://github.com/harshbhanushali26/finance-agent) | Terminal-based personal finance assistant — 8 natural language commands, zero cloud retention, all transaction data stays local | Python, Groq, JSON, CLI |
| [🎯 NextSteps](https://github.com/harshbhanushali26/NextSteps) | Resume-to-JD gap analyzer — parses unstructured resumes against job descriptions or URLs and outputs skill mapping + actionable roadmap | Python, Groq, Tavily |

---
## ⚙️ Technical Stack

### 🤖 AI & Agent Systems
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square&logoColor=white)
![Gemini API](https://img.shields.io/badge/Gemini_API-4285F4?style=flat-square&logo=google&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![MCP](https://img.shields.io/badge/Model_Context_Protocol-8B5CF6?style=flat-square&logoColor=white)
![RAG Architecture](https://img.shields.io/badge/RAG_Architecture-0ea5e9?style=flat-square&logoColor=white)

### 🗄️ Vector Storage & Embeddings
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat-square&logoColor=white)
![SentenceTransformer](https://img.shields.io/badge/SentenceTransformer-6C63FF?style=flat-square&logoColor=white)

### 🐍 Languages & Backend
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=sqlite&logoColor=white)

### 🛠️ Tools & Interfaces
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![uv](https://img.shields.io/badge/uv-000000?style=flat-square&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white)
![Rich CLI](https://img.shields.io/badge/Rich_CLI-1a1a2e?style=flat-square&logoColor=white)

---

## 🔨 Currently Building

**[Capsule](https://github.com/harshbhanushali26)** — A personal saved content manager built the right way: schema first, then logic, then interface.

- **Frontend:** Telegram bot + browser extension for saving content from anywhere
- **Backend:** FastAPI with async endpoints and Pydantic-validated request/response models
- **Processing:** Groq for content summarization and tagging at save-time
- **Storage:** SQLite for structured metadata + ChromaDB for semantic search across saved content

> Building this because every content manager I tried either had no AI or had AI bolted on. This one is designed around it.

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats-sigma-five.vercel.app/api?username=harshbhanushali26&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0f172a&title_color=38bdf8&icon_color=38bdf8&text_color=e2e8f0" width="48%"/>
  &nbsp;
  <img src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=harshbhanushali26&layout=compact&theme=tokyonight&hide_border=true&bg_color=0f172a&title_color=38bdf8&text_color=e2e8f0" width="48%"/>
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=harshbhanushali26&theme=tokyonight&hide_border=true&background=0f172a&stroke=38bdf8&ring=38bdf8&fire=38bdf8&currStreakLabel=38bdf8" width="60%"/>
</p>

---

## 🌐 Let's Connect

I'm actively looking for AI Engineer roles at startups where AI is the product, not a feature.
If that's you — or you know someone building that — reach out.

<p align="center">
  <a href="https://harshbhanushali26.github.io" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-Visit_Site-0ea5e9?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  &nbsp;&nbsp;
  <a href="https://www.linkedin.com/in/harshbhanushali0709/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  &nbsp;&nbsp;
  <a href="https://mail.google.com/mail/?view=cm&to=harshbhanu0709@gmail.com" target="_blank">
    <img src="https://img.shields.io/badge/Gmail-Inbox-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e3a8a,100:0f172a&height=70&section=footer"/>
</p>
