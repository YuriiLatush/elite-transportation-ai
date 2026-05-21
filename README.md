# Elite Transportation AI

Production AI system for a VIP transportation company in Los Angeles.
Handles lead qualification, pricing, and bookings via Telegram — deployed on Railway.

---

## The problem it solves

Transportation companies lose leads because no one responds at 2am.
This system qualifies every inquiry instantly, scores the lead, and alerts the sales team only when it's HOT.

---

## How it works
Telegram message
→ LangGraph router (pricing / booking / cancellation)
→ ChromaDB search (company knowledge, no hallucinations)
→ Lead scored: HOT / WARM / COLD
→ Response sent + saved to PostgreSQL
→ HOT lead → instant Telegram alert via n8n
---

## What's inside

| Component | What it does |
|---|---|
| LangGraph | Routes messages to the right agent |
| ChromaDB | Vector search over company knowledge base |
| Lead scoring | HOT / WARM / COLD with persistent rank (never downgrades) |
| PostgreSQL | Full conversation history, session memory |
| n8n webhook | Fires Telegram alert when lead score hits HOT |
| Railway | Deployed, running 24/7 |

---

## Built over 60 days

Started from `print("AI engineer journey started")`.
This is day 58 — the production version.

Timeline: RAG → multi-agent → LangGraph → PostgreSQL → deploy → this.

---

## Stack

Python 3.14 · OpenAI GPT-4o · LangGraph · ChromaDB · PostgreSQL · Railway · n8n · Telegram Bot API

---

## Author

**Yurii Latushkin** — [LinkedIn](https://linkedin.com/in/yurii-l-94082424b) · [GitHub](https://github.com/YuriiLatush)  
Marketing background. Building AI systems full time.
