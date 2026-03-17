# AI-Powered Retail Query System Using RAG

A production RAG chatbot that connects directly to a live retail 
database and answers customer queries in real time — product 
availability, pricing, stock levels — with zero hallucinations.

## What It Does

- Answers natural language queries about products instantly
- Pulls real-time data directly from SQLite database
- No static knowledge base — every answer grounded in live data
- Handles availability checks, pricing, and product details

## Tech Stack

- **LangChain** — RAG pipeline orchestration
- **Google PaLM LLM** — language understanding and response generation
- **SQLite** — live product database
- **Python** — backend logic

## Architecture
```
User Query → LangChain RAG Pipeline → SQLite Database Query
→ Context Retrieval → LLM Response Generation → Accurate Answer
```

## Key Features

- **Real-time retrieval** — queries live DB on every request
- **No hallucinations** — all answers grounded in actual inventory
- **Natural language interface** — customers ask in plain English
- **Few-shot learning** — response style tuned for retail context

## Example Queries
```
"Do you have blue t-shirts in size M?"
→ "Yes, we have 3 blue t-shirts in size M. Price: $24.99"

"What's the price of the Nike Air Max?"
→ "Nike Air Max is currently $89.99, available in sizes 8-12"
```

## Setup
```bash
git clone https://github.com/Fahd-8/AI-Powered-Retail-Query-System-Using-RAG
cd AI-Powered-Retail-Query-System-Using-RAG
pip install -r requirements.txt
python Product_Shop_Assistant.py
```

## Results

- Accurate real-time inventory responses
- Zero out-of-date information
- Natural conversational interface for non-technical users

---
Built by [Fahad Zaman](https://github.com/Fahd-8) — AI Engineer
```

---

Also add a `requirements.txt` file to the repo with:
```
langchain
google-generativeai
sqlite3
python-dotenv
