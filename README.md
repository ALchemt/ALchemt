# Andrey Ovsyannikov

**AI Engineer & Automation Builder** - building production-grade AI projects and automation systems under specific business pains, not pre-baked templates.

Started shipping in 2024. Builder before consultant: I'd rather ship a working v1 in two weeks and iterate from real usage than write a long proposal. Production-grade with real eval methodology so anyone can check the work.

---

## What I shipped (live, eval'd, code public)

### Policy Q&A Engine over GDPR + UK ICO regulations
For compliance teams burning hours on routine policy lookups. Production FastAPI service with hybrid retrieval (BM25 + dense, RRF fusion), citation-validated generation, full Langfuse observability. Documented finding: textbook RRF k=60 fails on small corpora.
- Live: **[alchemt-policy-qa-engine.hf.space](https://alchemt-policy-qa-engine.hf.space/)**
- Code: **[github.com/ALchemt/policy-qa-engine](https://github.com/ALchemt/policy-qa-engine)**
- Eval: 0% hallucination rate, factuality 1.32 / 2

### AI Recruiter Screening Tool
LangGraph agent doing JD-CV screening with RAG over JD corpus, LLM-as-judge eval, full Langfuse observability. 32-session eval with documented limitations.
- Live: **[alchemt-screening-tool.hf.space](https://alchemt-screening-tool.hf.space/)**
- Code: **[github.com/ALchemt/screening-tool](https://github.com/ALchemt/screening-tool)**

### RAG Document Q&A over AI Engineering Literature
Grounded question-answering over 25 AI engineering documents. LlamaIndex + ChromaDB + provider-agnostic generator (OpenRouter / Groq / HF Inference, swap with one env var).
- Live: **[alchemt-rag-qa.hf.space](https://alchemt-rag-qa.hf.space/)**
- Code: **[github.com/ALchemt/rag-qa](https://github.com/ALchemt/rag-qa)**
- Eval: 1.73 / 2 mean score, 0% hallucination rate, 60-question test set, split-judge methodology to control self-bias. Judge bugs left in the README on purpose.

### Reusable LLM Eval Framework
Regression harness for LLM systems. 3 test suites x N model configs, LLM-as-judge with JSON verdicts, Streamlit dashboard with diff between runs.
- Live: **[alchemt-llm-eval.hf.space](https://alchemt-llm-eval.hf.space/)**
- Code: **[github.com/ALchemt/llm-eval](https://github.com/ALchemt/llm-eval)**
- First benchmark: caught a 40-point reasoning gap between gpt-4o and gpt-4o-mini on the same prompts. That's a deployment decision, not a model choice.

### Voice Automation Receptionist (Proof-of-Concept)
For high-volume customer ops where one person still does what software should. Inbound call -> intent parsing -> CRM update -> customer confirmation. Stack: Vapi + n8n + Airtable. Replaces manual call coverage with a system that doesn't miss calls, doesn't sleep, scales without hiring.

### Multi-Agent Personal Operating System
Personal AI operating system handling my own daily ops: scheduled cron agents, voice input via Telegram, hook-driven safety layer, persistent memory across sessions, sub-agents for research, planning, code review, content writing. Runs unattended on a VPS. The hardest problem in agentic systems is keeping them honest under load - that's the angle I bring.

---

## Stack I use daily

**AI & RAG:** Python · LangChain · LangGraph · LlamaIndex · ChromaDB · FastAPI · Langfuse · Hybrid retrieval · LLM evaluation · Prompt engineering

**Workflow & Integration:** n8n · REST APIs · Webhooks · Airtable · Google Sheets

**Voice:** Vapi · Retell

**Infra:** Streamlit · HF Spaces · Docker · VPS deployment · Telegram Bot API

New tooling in this field shows up monthly - I learn whatever a project needs. The toolset isn't the value, the system that ships is.

---

## Looking for

Full-time remote role as **AI Engineer / AI Automation Engineer / LLM Engineer / Forward Deployed Engineer / Solutions Engineer (AI)**. Also taking 1-2 selective contract engagements per month.

Open to US · UK · EU · Singapore · Vietnam timezones.

**Contact:** andrey2014536@gmail.com | [LinkedIn](https://www.linkedin.com/in/andrey-ovsyannikov-12a5b2404/)
