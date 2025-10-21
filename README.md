<!-- Banner -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0ea5e9,100:22c55e&height=200&section=header&text=Youssef%20Ismail&fontSize=42&fontAlignY=35&animation=fadeIn" alt="Youssef Ismail banner" />
</p>

<!-- Typing headline -->
<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Inter&weight=700&size=26&duration=2600&pause=800&center=true&vCenter=true&width=820&lines=Agentic+systems+(LangGraph)+%7C+RAG+(retrieval+%2B+reranking+%2B+evaluation);Practical+AI+apps+with+observability+and+guardrails;Currently+learning+AWS+deployments+and+API+design" alt="typing headline"/>
  <br/>
  <!-- Focus / Learning badges -->
  <img alt="focus-agents" src="https://img.shields.io/badge/Focus-LangGraph%20Agents-0f172a?labelColor=0f172a&color=0ea5e9">
  <img alt="focus-rag" src="https://img.shields.io/badge/Focus-RAG%20Pipelines-0f172a?labelColor=0f172a&color=22c55e">
  <img alt="learning" src="https://img.shields.io/badge/Learning-AWS%20Deployments%20%26%20APIs-0f172a?labelColor=0f172a&color=f59e0b">
</div>

---

### 👋 About me
I build **agentic** and **RAG** systems that are **observable**, **eval-driven**, and **easy to ship**.  
Right now I’m exploring **AWS serverless** (API Gateway · Lambda · S3 · Bedrock) and **API design** (FastAPI/REST).

- 🔭 Working on: multi-agent flows; RAG with reranking & faithfulness checks  
- 🌱 Learning: IaC patterns, auth/rate-limits, request/response contracts  
- 💬 Ask me about: LangGraph agents, RAG, Streamlit prototypes  
- 📫 Contact: <your-email@example.com>

---

### 🚀 Featured work (pin these below)
- **Gold Price Reporter** — LangGraph multi-agent flow (Arabic UI, Streamlit)
- **Medical RAG Assistant** — Hybrid retrieval + evaluation harness (LitQA-style)
- **News Research Tool** — URL → embeddings → Q&A with sources (FAISS + Streamlit)
- **Chat with Search** — ReAct agent choosing web/arXiv/Wikipedia (Groq + Streamlit)
- **Chat with PDF** — Bedrock (Titan + FAISS) with Claude/Mistral toggle
- **Chat with SQL DB** — SQL agent over SQLite/MySQL with Groq

> Profile → **Customize profile** → **Pinned repositories** → select 4–6 from the list.
 Optional: repo cards (uncomment + set the exact repo slugs)
<div align="center">
  <a href="https://github.com/youssef2323/<repo_slug_1>"><img height="132" src="https://github-readme-stats.vercel.app/api/pin/?username=youssef2323&repo=<repo_slug_1>&theme=transparent&hide_border=true"></a>
  <a href="https://github.com/youssef2323/<repo_slug_2>"><img height="132" src="https://github-readme-stats.vercel.app/api/pin/?username=youssef2323&repo=<repo_slug_2>&theme=transparent&hide_border=true"></a>
</div>

---

### 🧩 Agentic RAG — quick view
```mermaid
flowchart LR
  A[User] -->|question| R(Agent Router)
  R -->|needs docs| RET[Retriever]
  RET --> RR[Reranker]
  RR --> L[LLM Draft]
  L --> E{Evaluators}
  E -->|faithfulness OK| F[Final Answer + Sources]
  E -->|not OK| R
  R -->|needs tool| T[Tools: Search · SQL · Web]
  T --> R

