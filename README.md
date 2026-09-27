<img src="assets/terminal.svg" width="100%" alt="Rishav Raj — full-stack engineer" />

Hi, I'm **Rishav** — a full-stack engineer who got tired of demos that die the moment real data shows up.

By day I build and run production services: Next.js + TypeScript frontends, Python backends. The rest of the time I'm retooling into **AI engineering** — properly, not tutorial-style: retrieval quality you can *measure*, agents that cite their sources, and evals that block a bad PR before it merges.

I like problems where the hard part is honesty. A 300-page SEC filing that *almost* answers your question is more dangerous than one that clearly doesn't — so my projects are built around knowing the difference.

## ☕ Loved something here? Buy me a chai

If a project, a post, or a script of mine saved you an evening — a chai is the simplest way to say *"it worked"*. Pay what it's worth to you.

<div align="center">
  <a href="https://iamrishavraj1.com/#chai">
    <img src="assets/upi-qr.png" width="170" alt="UPI QR — scan to buy Rishav a chai" />
  </a>
  <br/>
  <sub>scan with any UPI app · <code>rishavraj2000@yescred</code></sub>
</div>

## 🔗 Quick links

<div align="center">
  <a href="https://calendar.google.com/calendar/appointments/schedules/AcZssZ3kA3Y1K7TJHi3QfMzpYdrI58PUyLqkXSbcx34Dfn5VQiBcoy3CHHkBwRSqUYuE6Cidih66Ahns?gv=true"><img src="https://img.shields.io/badge/Book%20a%20call-30%20min%20·%20Google%20Calendar-1F6FEB?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a call" /></a>
  <a href="https://iamrishavraj1.com/resume"><img src="https://img.shields.io/badge/R%C3%A9sum%C3%A9-view%20%2F%20save%20PDF-39D2C0?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="Résumé" /></a>
  <a href="https://iamrishavraj1.com"><img src="https://img.shields.io/badge/Website-iamrishavraj1.com-1F6FEB?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website" /></a>
  <a href="https://x.com/iamrishavraj1"><img src="https://img.shields.io/badge/X-%40iamrishavraj1-000000?style=for-the-badge&logo=x&logoColor=white" alt="X" /></a>
  <a href="mailto:iamrishavraj1@gmail.com"><img src="https://img.shields.io/badge/Email-iamrishavraj1%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</div>

## Building in public

### 🚧 [fin-research-agent](https://github.com/iamrishavraj1/fin-research-agent) — AI research assistant over SEC filings

Ask *"Which company grew revenue fastest after its 2023 acquisition?"* → get a **cited answer**, or an honest *"the filings don't say."*

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

- Hybrid retrieval (BM25 + pgvector) — measured with recall@k and MRR, not vibes
- A raw, no-framework tool-using agent: document search, SQL over financials, calculator
- An eval suite that gates CI — the part most RAG repos skip
- Architecture, docs and eval design are up; code lands week by week

### ✅ [interview-buddy](https://github.com/iamrishavraj1/interview-buddy) — mock interviews that run 100% on my Mac

Speaks questions out loud (Ollama · qwen3:14b), listens to spoken answers (faster-whisper), and coaches: score /10, filler-word counter, STAR-mode feedback. ₹0 per session, works offline. The interesting bit is the design — the **server** runs the interview (question order, when to push), the LLM only converses. Deterministic control, natural feel.

## How I work

- **Measure, then ship.** Every retrieval or prompt change runs the evals.
- **No framework magic in the core loop.** If I can't explain a line in an interview, it doesn't ship.
- **Boring code, interesting products** — in that order.

## 🏅 Track record

- **Dharmveer Award** — High Integrity & Ownership, for delivery quality and scalable architecture
- **Pull Shark ×2 · YOLO** — GitHub achievements for merged contributions
- **15,000+ reads** across technical writing on [dev.to](https://dev.to/iamrishavraj1), [Hashnode](https://iamrishavraj1.hashnode.dev) and [Medium](https://iamrishavraj1.medium.com)

## Stack

**Frontend** Next.js · React · TypeScript · Tailwind &nbsp;|&nbsp; **Backend** Python · FastAPI · Postgres + pgvector &nbsp;|&nbsp; **Ops** Docker · GitHub Actions &nbsp;|&nbsp; **AI** Ollama · OpenAI-compatible APIs · faster-whisper

---

*Built by hand — no framework for the profile, Next.js for [the site](https://iamrishavraj1.com).*
