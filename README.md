<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:1e3a8a&height=200&section=header&text=Harsh%20Bhanushali&fontSize=40&fontColor=ffffff&animation=fadeIn&fontAlignY=35"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1000&color=38BDF8&center=true&vCenter=true&width=700&lines=Agentic+AI+Developer;RAG+Pipelines+%7C+LLM+Orchestration;Multi-Agent+Systems+%7C+Cost-Aware+AI;Groq+%7C+Gemini+%7C+ChromaDB+%7C+Streamlit;Open+to+AI+Engineer+Roles" />
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
  <a href="https://mail.google.com/mail/?view=cm&to=harshbhanu0709@gmail.com" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/Gmail-harshbhanu0709-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
</p>

---

## 🧠 About Me

I build autonomous AI systems in Python — deliberate architecture, minimal dependencies, full control over every layer.

My work spans **RAG pipelines** with ChromaDB and SentenceTransformer, **multi-agent orchestration** with complexity-based model routing, cost-aware LLM APIs (Groq, Gemini), and modular agent design. I also have hands-on production engineering experience — shipped 3 enterprise web applications during my internship, improving workflow efficiency by 30%.

> *"I don't use frameworks as a crutch — I use them deliberately, only where they earn their place."*

---

## 🚀 Shipped Projects

| Project | Description | Stack |
|--------|-------------|-------|
| 🧠 **[hArI](https://github.com/harshbhanushali26/hArI)** | RAG document intelligence app — upload PDFs, ask questions, get grounded answers with source citations. Production-deployed. | Groq · ChromaDB · SentenceTransformer · Streamlit |
| 🔬 **[Multi-Agent Research Pipeline](https://github.com/harshbhanushali26/research-pipeline)** | CLI pipeline with 6 specialized agents — Search, Scrape, Summarize, Critique, Synthesize, Supervise. Complexity-based model routing with Groq/Gemini fallback. | Groq · Gemini · DuckDuckGo · Rich |
| 🤖 **[AI Agent Engine](https://github.com/harshbhanushali26/ai-agent-engine)** | 4-layer autonomous agent — cache → pattern router → RAG → LLM. ~80% queries resolved with 0 LLM calls. Per-session cost ~$0.0005. | Gemini · ChromaDB · SentenceTransformer |
| 💰 **[Finance Agent CLI](https://github.com/harshbhanushali26/expense-tracker)** | 8 natural-language commands for personal finance — budgets, summaries, dashboards. Fully offline beyond Groq API. | Groq · Python · OOP · JSON |
| 🎯 **[NextSteps](https://github.com/harshbhanushali26/nextsteps)** | Career planning AI app — upload resume + JD/URL → gap analysis, skill mapping, personalized roadmap. | Groq · Tavily · Python |

---



## 🏗️ Featured Projects


### 🧠 hArI — RAG Document Intelligence
Production-deployed app for intelligent PDF Q&A with grounded answers and source citations.

- Cosine similarity retrieval with `SCORE_THRESHOLD=0.35` — no hallucinated sources
- Intent detection routes queries: conversational → RAG → LLM fallback
- Deduped source citations with chunk-level cosine filtering
- `strip_thinking()` post-processing for clean, structured responses
- Stack: Groq (llama-4-scout-17b), ChromaDB, SentenceTransformer (all-MiniLM-L6-v2), PyMuPDF, Streamlit, uv

🔗 [View Repository](https://github.com/harshbhanushali26/hArI)

---

### 🔬 Multi-Agent Research Pipeline
CLI-based autonomous research system with 6 specialized agents and quota-aware model routing.

- Supervisor → Search → Scrape → Summarize → Critique → Synthesize pipeline
- Complexity-based routing: Groq (llama-3.3-70b) primary, Gemini (gemini-3-flash-preview) fallback
- Human-in-the-loop checkpoints with Rich terminal UI
- Stack: Groq, Gemini, DuckDuckGo, Rich, Python

🔗 [View Repository](https://github.com/harshbhanushali26/research-pipeline)

---

### 🎯 NextSteps — Career Path AI
AI-powered career planning app — paste a resume and JD or URL, get a full gap analysis and roadmap.

- Parses unstructured resume + job formats with no hardcoded assumptions
- Delivers skill mapping, gap analysis, and personalized roadmap in under 5–8 minutes
- Clean separation: parsing → analysis → output generation
- Stack: Groq, Tavily, Python

🔗 [View Repository](https://github.com/harshbhanushali26/NextSteps)

---



### 🤖 AI Agent Engine
Production-grade autonomous agent built entirely from scratch in Python.

- 4-layer pipeline: cache → pattern router → RAG → LLM
- ~80% of queries resolved with **0 LLM calls** via deterministic routing
- ChromaDB + SentenceTransformer RAG with **~30ms** semantic search latency
- Planner → Validator → Executor → Responder structured pipeline
- Per-session cost **~$0.0005** with daily quota enforcement
- Stack: Python 3.11+, Gemini API, ChromaDB, SentenceTransformer, DuckDuckGo Search, Open-Meteo

🔗 [View Repository](https://github.com/harshbhanushali26/ai-agent-engine)



---


### 💰 Finance Agent (CLI)
Standalone CLI finance agent powered by Groq — switched from Gemini after hitting quota limits, found better speed and reliability for this use case.

- 8 natural-language commands: add, update, delete, summaries, budgets, dashboards
- Zero code duplication — reuses Expense Tracker classes (~60% dev time reduction)
- Config-driven per-category monthly budget system
- Fully offline storage — no external dependency beyond Groq API
- Stack: Python, Groq API, OOP, JSON storage, CLI

🔗 [View Repository](https://github.com/harshbhanushali26/expense-tracker)

---

### 🧾 Expense Tracker
Multi-user expense tracker with secure auth and offline JSON storage.

- Handles **1,000+ records** efficiently without a database
- **40% code complexity reduction** via OOP design patterns
- Daily/monthly analytics with real-time dashboards
- Foundation reused entirely for Finance Agent — zero duplication

🔗 [View Repository](https://github.com/harshbhanushali26/expense-tracker)

---

### ☕ BrewOps — Café Management CLI
Modular Python + Rich CLI system for full café operations.

- 9 independent modules: auth, menu, orders, analytics, session management
- Secure password hashing/salting + **30-min auto session timeout** with 2-level warnings
- 7+ operational features across admin & customer portals
- Full order lifecycle + daily/monthly analytics dashboards

🔗 [View Repository](https://github.com/harshbhanushali26/BrewOps)

---

## ⚙️ Technical Stack

### AI & Agents
![Gemini API](https://img.shields.io/badge/Gemini_API-4285F4?style=flat-square&logo=google&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat-square&logoColor=white)
![SentenceTransformer](https://img.shields.io/badge/SentenceTransformer-6C63FF?style=flat-square&logoColor=white)
![RAG](https://img.shields.io/badge/RAG-0ea5e9?style=flat-square&logoColor=white)
![LLM Orchestration](https://img.shields.io/badge/LLM_Orchestration-1D9E75?style=flat-square&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

### Languages & Core
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

### ML Libraries
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)

### Web & Backend
![ASP.NET](https://img.shields.io/badge/ASP.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![HTML](https://img.shields.io/badge/HTML-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=flat-square&logo=css3&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white)

### Tools
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)

---

## 📚 Currently Learning

<table>
  <tr>
    <td align="center">
      <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/><br/>
      <sub>Stateful multi-agent workflows</sub>
    </td>
    <td align="center">
      <img src="https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white"/><br/>
      <sub>Workflow automation</sub>
    </td>
    <td align="center">
      <img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logoColor=white"/><br/>
      <sub>Local LLM inference</sub>
    </td>
  </tr>
</table>

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=harshbhanushali26&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0f172a&title_color=38bdf8&icon_color=38bdf8&text_color=e2e8f0" width="48%"/>
  &nbsp;
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=harshbhanushali26&layout=compact&theme=tokyonight&hide_border=true&bg_color=0f172a&title_color=38bdf8&text_color=e2e8f0" width="48%"/>
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=harshbhanushali26&theme=tokyonight&hide_border=true&background=0f172a&stroke=38bdf8&ring=38bdf8&fire=38bdf8&currStreakLabel=38bdf8" width="60%"/>
</p>

---

## 🌐 Connect

<p align="center">
  <a href="https://harshbhanushali26.github.io" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-Visit-0ea5e9?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  &nbsp;&nbsp;
  <a href="https://www.linkedin.com/in/harshbhanushali0709/" target="_blank">
    <img src="https://skillicons.dev/icons?i=linkedin" height="50"/>
  </a>
  &nbsp;&nbsp;
<a href="https://mail.google.com/mail/?view=cm&to=harshbhanushali26@gmail.com" target="_blank" rel="noopener noreferrer">
    <img src="https://skillicons.dev/icons?i=gmail" height="50"/>
  </a>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e3a8a,100:0f172a&height=70&section=footer"/>
</p>
