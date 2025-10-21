<!-- HERO -->
<div align="center">
  <!-- Animated headline -->
  <img src="https://readme-typing-svg.demolab.com?font=Inter&weight=700&size=28&duration=2600&pause=800&center=true&vCenter=true&width=820&lines=Youssef+Ismail;LangGraph+multi-agent+systems;RAG%3A+retrieval+%2B+reranking+%2B+evaluation;Building+practical+AI+apps;Learning+AWS+deployments+and+APIs" alt="typing headline" />
  <br/>

  <!-- Focus badges -->
  <img alt="focus-agents" src="https://img.shields.io/badge/Focus-LangGraph%20Agents-0f172a?labelColor=0f172a&color=0ea5e9">
  <img alt="focus-rag" src="https://img.shields.io/badge/Focus-RAG%20Pipelines-0f172a?labelColor=0f172a&color=22c55e">
  <img alt="learning" src="https://img.shields.io/badge/Learning-AWS%20Deployments%20%26%20APIs-0f172a?labelColor=0f172a&color=f59e0b">
</div>

---

### About me
I build **agentic** and **RAG** systems that are **observable**, **eval-driven**, and **easy to ship**.  
Right now, I’m exploring **AWS serverless** (API Gateway · Lambda · S3 · Bedrock) and **API design** (FastAPI/REST).

- 🔭 Working on: LangGraph multi-agent flows; RAG with reranking & faithfulness checks  
- 🌱 Learning: AWS deployments & IaC templates; auth, rate-limits, request/response contracts  
- 💬 Ask me about: LangGraph agents, RAG, Streamlit prototypes  
- 📫 Contact: <your-email>  

---

### Featured work
> Pin these on your profile (Profile → Customize profile → Pinned repositories)

- **Gold Price Reporter** — LangGraph multi-agent flow (Arabic UI, Streamlit)  
- **Medical RAG Assistant** — Hybrid retrieval + evaluation harness (LitQA-style)  
- **News Research Tool** — URL → embeddings → Q&A with sources (FAISS + Streamlit)  
- **Chat with Search** — ReAct agent choosing web/arXiv/Wikipedia (Groq + Streamlit)  
- **Chat with PDF** — Bedrock (Titan + FAISS), Claude/Mistral toggle  
- **Chat with SQL DB** — SQL agent over SQLite/MySQL with Groq  
<!-- Optional repo cards (uncomment + set repo slugs)
<div align="center">
  <a href="https://github.com/youssef2323/<repo1>"><img height="130" src="https://github-readme-stats.vercel.app/api/pin/?username=youssef2323&repo=<repo1>&theme=transparent&hide_border=true"></a>
  <a href="https://github.com/youssef2323/<repo2>"><img height="130" src="https://github-readme-stats.vercel.app/api/pin/?username=youssef2323&repo=<repo2>&theme=transparent&hide_border=true"></a>
</div>
-->

---

### Agentic RAG at a glance
```mermaid
flowchart LR
  A[User] -->|question| B(Agent: Router)
  B -->|needs docs| C[Retriever]
  C -->|top-k chunks| D[Reranker]
  D --> E[LLM: Answer Draft]
  E --> F{Evaluator Nodes}
  F -->|faithfulness OK| G[Final Answer + Sources]
  F -->|not OK| B
  B -->|needs tool| T[Tools: Search · SQL · Web]
  T --> B

