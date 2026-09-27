<!-- Profile README for github.com/iamrishavraj1 — paste into the repo named exactly `iamrishavraj1` -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6&height=180&section=header&text=Rishav%20Raj&fontSize=42&fontColor=ffffff&animation=fadeIn&desc=Full-Stack%20Engineer%20%C2%B7%20building%20AI%20agents%20in%20public&descSize=17&descAlignY=70&descAlignX=center" alt="Rishav Raj" />

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=19&pause=1200&color=58A6FF&center=true&vCenter=true&width=620&lines=Next.js+and+TypeScript+by+day;AI+engineer+by+night:+RAG,+agents,+evals;Building+in+public:+metrics+over+vibes" alt="typing" />
</div>

## 👋 Hey, I'm Rishav

**Full-Stack Engineer @ Virohan** — I ship Next.js + TypeScript frontends for a living,
and I'm on a deliberate path into **AI engineering**. Not the "called the OpenAI API once"
kind — the kind with retrieval metrics, eval suites that gate CI, and agents that admit
what they don't know.

What I optimize for:

- 📏 **Measure, then ship** — recall@k before vibes
- 🧱 Systems that survive contact with real, messy data (300-page SEC filings, anyone?)
- ✍️ Clean, boring code the next engineer can actually read

## 🔭 What I'm building

### 🏗️ [fin-research-agent](https://github.com/iamrishavraj1/fin-research-agent) — AI research assistant over SEC filings `building in public`

Ask *"which company grew revenue fastest after its 2023 acquisition?"* and get a cited
answer — or an honest "the filings don't say."

```mermaid
flowchart LR
    E["SEC EDGAR<br/>10-K · 10-Q · 8-K"] --> I["Ingestion<br/>parse → chunk → embed"]
    I --> DB[("Postgres<br/>+ pgvector")]
    DB --> H["Hybrid retrieval<br/>BM25 + vector → rerank"]
    DB --> Q["SQL tool<br/>structured financials"]
    H --> A["Agent"]
    Q --> A
    A --> O["Answer with citations<br/>or honest refusal"]
    V["Evals — golden set<br/>recall@k · MRR · CI-gated"] -.-> A
```

- **Hybrid retrieval** — BM25 + pgvector, fused and reranked, *measured* with recall@k and MRR
- **Tool-using agent** — document search, SQL over extracted financials, calculator; every claim carries a citation
- **Evals as a first-class artifact** — a golden question set scored on every PR, gating CI. Almost nobody builds this; every team wants it
- **Production concerns** — streaming, cost/latency tracking, tracing, prompt-injection defense

![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-async-009688?style=flat-square&logo=fastapi&logoColor=white)
![Postgres](https://img.shields.io/badge/PostgreSQL-pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-compose-2496ED?style=flat-square&logo=docker&logoColor=white)
![pytest](https://img.shields.io/badge/evals-CI--gated-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

### ✅ [interview-buddy](https://github.com/iamrishavraj1/interview-buddy) — a voice interview coach that runs 100% on my Mac `shipped`

It asks questions **out loud**, listens to spoken answers, and coaches — filler-word
counter, score /10, STAR-mode feedback, transcripts. Powered by Ollama (qwen3:14b) +
faster-whisper, so practice costs ₹0 and works offline.

![FastAPI](https://img.shields.io/badge/FastAPI-server-009688?style=flat-square&logo=fastapi&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-qwen3:14b-111111?style=flat-square&logo=ollama&logoColor=white)
![Whisper](https://img.shields.io/badge/faster--whisper-STT-8A2BE2?style=flat-square&logo=openai&logoColor=white)

## 🧰 The toolbox

<div align="center">
  <img src="https://skillicons.dev/icons?i=ts,react,nextjs,tailwind,python,fastapi,postgres,docker,githubactions,git,html,css&perline=6" alt="stack" />
</div>

## 📊 GitHub stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=iamrishavraj1&show_icons=true&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=1f6feb&text_color=c9d1d9&count_private=true" alt="GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=iamrishavraj1&layout=compact&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9&langs_count=8" alt="Top languages" />
</p>

## 🌱 Right now

- 🧪 going deep on **evals & RAG quality** — golden sets, regression gating, retrieval metrics
- 🏗️ studying **system design** — consistency, caching, rate limiting
- 🎙️ dogfooding interview-buddy daily (it roasts my filler words)

## 📮 Reach me

<div align="center">
  <a href="mailto:iamrishavraj1@gmail.com"><img src="https://img.shields.io/badge/Email-iamrishavraj1%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://iamrishavraj1.com"><img src="https://img.shields.io/badge/Website-iamrishavraj1.com-1F6FEB?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website" /></a>
  <a href="https://x.com/iamrishavraj1"><img src="https://img.shields.io/badge/X-%40iamrishavraj1-000000?style=for-the-badge&logo=x&logoColor=white" alt="X" /></a>
</div>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6&height=110&section=footer" />
