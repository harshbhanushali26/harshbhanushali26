<p align="center">  
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:1e3a8a&height=180&section=header&text=Harsh%20Bhanushali&fontSize=38&fontColor=ffffff&animation=fadeIn&fontAlignY=35"/>  
</p>

<div align="center">  
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=19&pause=800&speed=40&color=38BDF8&center=true&vCenter=true&width=750&lines=AI+Systems+%26+Autonomous+Agents+Engineer;Architecture-First%3A+State+Then+Code;Building+Waypoint+%E2%80%94+Autonomous+Trip+Planning+AI+Agent;Deterministic+Workflows+%2B+Multi-Agent+Systems;Open+to+AI+Engineer+Roles" />  
</div>

<p align="center">  
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>  
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangGraph"/>  
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangChain"/>  
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI"/>  
  <img src="https://img.shields.io/badge/RAG-0284C7?style=for-the-badge&logoColor=white" alt="RAG"/>  
  <img src="https://img.shields.io/badge/MCP-8B5CF6?style=for-the-badge&logoColor=white" alt="MCP"/>  
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/>  
</p>

<!-- <p align="center">  
  <img src="https://skillicons.dev/icons?i=python,fastapi,postgres,supabase,docker,git,github,sqlite" alt="Core engineering stack"/>  
</p> -->

<p align="center">  
  <sub>State → Route → Execute → Validate → Observe</sub>  
</p>

<p align="center">  
  <a href="https://harshbhanushali26.github.io" target="_blank">  
    <img src="https://img.shields.io/badge/Portfolio-harshbhanushali26.github.io-0284c7?style=flat-square&logo=googlechrome&logoColor=white"/>  
  </a>  
  &nbsp;  
  <a href="https://www.linkedin.com/in/harshbhanushali0709/" target="_blank">  
    <img src="https://img.shields.io/badge/LinkedIn-harshbhanushali0709-0077B5?style=flat-square&logo=linkedin&logoColor=white"/>  
  </a>  
  &nbsp;  
  <a href="mailto:harshbhanu0709@gmail.com" target="_blank">  
    <img src="https://img.shields.io/badge/Email-Direct%20Inquiry-EA4335?style=flat-square&logo=gmail&logoColor=white"/>  
  </a>  
</p>

<p align="center">  
  <code>⚡ <b>Status:</b> Actively interviewing for AI Engineer roles (India / Remote)</code>  
</p>

---

## 🧩 Core Capabilities


 
<div align="center">
<code>Multi-Agent Systems</code> <code>Stateful Workflows</code> <code>Deterministic Routing</code> <code>Hybrid RAG</code> <code>Tool Execution</code> <code>HITL</code> <code>Cost-Aware AI</code> <code>Evaluation & Guardrails</code>
</div>


---

## ⚡ Engineering Philosophy

> *"The architecture meeting you skip always becomes the non-deterministic bug you can't trace in production."*

I build reliable LLM applications, multi-agent orchestrations, and hybrid retrieval systems. My approach prioritizes explicit state machines, strict context boundaries, cost-guardrail routing, and deterministic evaluation layers before relying on raw LLM inference.

---

## 🚀 Active Build

### 🧭 [Waypoint — Multi-Agent AI Trip Planner](https://github.com/harshbhanushali26/waypoint)

*Every great journey starts with a Waypoint. A user describes a trip through a structured form; a graph of LangGraph agents plans transport, lodging, activities, and budget; the system produces a day-by-day itinerary; and the user refines it through a chat-based review loop before finalizing.*

**User flow:** `Form fill → Trip session starts → Planning runs → Human review (chat loop) → Final itinerary`

- **5-Agent Graph:** `Concierge` normalizes raw form input → `Planner` decides search priority → `Budget` sums cost against stated budget → `Itinerary` composes the day-by-day plan → `Critic` interprets edit requests during review. Human-in-the-loop gate at `human_review` node.
- **Write-Safe State:** TypedDict `TripState` — single source of truth with separate top-level keys per tool result (not a grouped dict) for conflict-free parallel fan-out. Postgres checkpointer (`langgraph-checkpoint-postgres`) persists paused graph state so a session survives refresh/restart.
- **7 Mechanical Tool Nodes:** `search_flights`, `search_trains`, `search_buses`, `search_cars`, `search_hotels`, `search_activities`, `get_weather` — no LLM calls, staged dummy → free API (Tavily) → MCP.
- **First Framework Project:** LangGraph + LangChain orchestration instead of hand-rolled agents — deliberate framework adoption with full understanding of the graph execution model underneath.
- **Stack:** `Python` • `LangGraph` • `LangChain` • `FastAPI` • `Postgres` • `SQLAlchemy` • `Alembic` • `Pydantic` • `Tenacity` • `Groq` (`gpt-oss-120b`) • `OpenAI` (fallback) • `Tavily` • `MCP`

---

## 🛠️ Featured Systems & Architectures

<table>  
<tr>  
<td valign="top" width="50%">

### 💸 [FinOS — AI Finance Platform](https://github.com/harshbhanushali26/finos)

Full-stack financial OS combining an interactive analytics dashboard with a conversational agent engine — both writing to the same SQLite store.

- **Zero-Cost Hybrid Router:** Resolves ~60% of deterministic queries via pattern matching at $0 LLM cost; streams fallbacks via Groq + SSE.
- **Predictive Analytics:** Financial health scoring, spending trajectory forecasts, budget threshold alerts.
- **Hardened Auth:** bcrypt with session tokens and CLI-based recovery.

`Python` • `FastAPI` • `SQLModel` • `Groq` • `SSE` • `SQLite`

</td>  
<td valign="top" width="50%">

### 🧠 [hArI v2 — Document Intelligence](https://github.com/harshbhanushali26/hArI)

High-precision RAG engine rebuilt from a single-store ChromaDB prototype into a hybrid-search, multi-user system.

- **Hybrid Retrieval:** Dense pgvector similarity coupled with tsvector full-text search via a custom Supabase RPC.
- **Sandboxed Analytics:** DuckDB SQL engine replacing `pandas.exec()` for safe multi-CSV queries.
- **Multi-User:** Supabase Auth, per-user chat persistence, citation UI with telemetry feedback.

`Python` • `Supabase` • `pgvector` • `DuckDB`

</td>  
</tr>  
<tr>  
<td valign="top" width="50%">

### 🤖 [AI Agent Engine](https://github.com/harshbhanushali26/ai-agent-engine)

Modular 4-layer query routing and execution system designed to eliminate unconstrained agent loops.

- **Deterministic Pre-Filtering:** ChromaDB + SentenceTransformer semantic layer resolves ~80% of repeat queries locally at ~30ms.
- **Guardrail Architecture:** Planner → Validator → Executor → Responder with hard session token and quota cutoffs.
- **Cost Efficiency:** Per-session cost ~$0.0005.

`Python` • `Gemini API` • `ChromaDB` • `SentenceTransformer`

</td>  
<td valign="top" width="50%">

### 🔬 [Research Pipeline](https://github.com/harshbhanushali26/research-pipeline)

6-agent supervisor workflow orchestrating deep, multi-hop web research with zero context degradation.

- **Stateful Segregation:** Supervisor → Search → Scraper → Summarizer → Critic → Synthesizer.
- **Model Routing:** Groq (`llama-3.3-70b`) primary  Gemini (`gemini-2.0-flash`) fallback, complexity-based.
- **HITL Control Gates:** Human-in-the-Loop review checkposts with multi-provider fallback layers.

`Python` • `Groq` • `Gemini API` • `Rich CLI`

</td>  
</tr>  
<tr>  
<td colspan="2" valign="top">

### 🎯 [NextSteps — Career Gap Engine](https://github.com/harshbhanushali26/NextSteps)

Actionable talent intelligence pipeline translating JD criteria into verified technical roadmaps.

- **Semantic Parsing:** Unstructured resume extraction matched against live JD requirements or URLs.
- **Targeted Synthesis:** Maps identified skill discrepancies directly to granular learning modules.
- **Clean Pipeline:** Parse → analyze → output — no hardcoded resume/JD assumptions.

`Python` • `FastAPI` • `Groq` • `Tavily`

</td>  
</tr>  
</table>

---

## 🗃️ Tooling & Protocol Implementations

| Repository | Focus & Architecture | Primary Tech |
|:---|:---|:---|
| [**🔌 DevMind — MCP Server**](https://github.com/harshbhanushali26/mcp-implementations) | Secure Model Context Protocol tool server exposing 6 developer tools — file ops, Python execution, JSON utilities — with human-gated execution boundaries. | `MCP SDK` • `Python` • `tiktoken` |
| [**🗄️ LangGraph Parallel SQL Runner**](https://github.com/harshbhanushali26/langgraph-parallel-sql) | Graph-governed parallel SQL executor via LangGraph's Send API, with automated syntax validation and pre-execution human review. | `LangGraph` • `Groq` • `SQLite` |

---

## 💻 Tech Stack


### 🤖 AI & Agent Systems

![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square&logo=groq&logoColor=white) ![Gemini API](https://img.shields.io/badge/Gemini_API-1C69E0?style=flat-square&logo=googlegemini&logoColor=white) ![LangGraph](https://img.shields.io/badge/LangGraph-1A1A1A?style=flat-square&logoColor=white) ![MCP](https://img.shields.io/badge/Model_Context_Protocol-6E45C2?style=flat-square&logoColor=white) ![RAG](https://img.shields.io/badge/RAG_Architecture-4493FF?style=flat-square&logoColor=white)

### 🗄️ Data & Vector Storage

![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white) ![pgvector](https://img.shields.io/badge/pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black) ![ChromaDB](https://img.shields.io/badge/ChromaDB-FF4F00?style=flat-square&logoColor=white) ![SentenceTransformer](https://img.shields.io/badge/SentenceTransformer-7F52FF?style=flat-square&logoColor=white)

### 🐍 Languages & Backend

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logoColor=white) ![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logoColor=white)

### 🛠️ Tools & Interfaces

![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![uv](https://img.shields.io/badge/uv-DE5FE9?style=flat-square&logoColor=white) ![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white) ![Rich CLI](https://img.shields.io/badge/Rich_CLI-7C3AED?style=flat-square&logoColor=white)

---

## 📈 Activity & Metrics

<div align="center">  
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=harshbhanushali26&theme=tokyonight&hide_border=true&background=090d16&ring=38bdf8&fire=38bdf8&currStreakLabel=38bdf8&sideLabels=94a3b8" height="170" alt="GitHub Streak">
  <br>
</div>

---

<div align="center">  
  <p><b>Interested in collaborating or discussing AI Engineer opportunities?</b></p>  
  <a href="mailto:harshbhanu0709@gmail.com">  
    <img src="https://img.shields.io/badge/Get_in_Touch-harshbhanu0709@gmail.com-0284c7?style=for-the-badge&logo=gmail&logoColor=white"/>  
  </a>  
</div>

<p align="center">  
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:1e3a8a&height=60&section=footer"/>  
</p>
