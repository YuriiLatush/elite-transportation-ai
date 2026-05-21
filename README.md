# Elite Transportation AI 🚗

![Python](https://img.shields.io/badge/Python-3.14-blue?style=for-the-badge&logo=python)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT4o-black?style=for-the-badge&logo=openai)
![LangGraph](https://img.shields.io/badge/LangGraph-Latest-orange?style=for-the-badge)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-blue?style=for-the-badge&logo=postgresql)
![ChromaDB](https://img.shields.io/badge/ChromaDB-VectorDB-green?style=for-the-badge)
![Railway](https://img.shields.io/badge/Railway-Deployed-purple?style=for-the-badge)

AI sales agent for a VIP transportation company in Los Angeles. Built to handle client inquiries, qualify leads, and calculate pricing automatically.

---

## What it does

- Routes every message to the right agent (pricing, booking, cancellation)
- Searches a vector database before answering — no hallucinations
- Scores leads automatically: HOT / WARM / COLD
- Saves full conversation history to PostgreSQL
- Sends instant Telegram alerts when a lead goes HOT

---

## Architecture
User Message
↓
LangGraph Classifier
↓
PRICING / BOOKING / CANCEL
↓
RAG Search (ChromaDB)
↓
Answer + Lead Score
↓
PostgreSQL (saved)
---

## Stack

Python · OpenAI · LangGraph · ChromaDB · PostgreSQL · Railway · n8n · Telegram Bot API

---

## Built by

[Yurii Latushkin](https://linkedin.com/in/yurii-l-94082424b) — Marketing background, building AI systems full time.
