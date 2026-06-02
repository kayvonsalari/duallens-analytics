# DualLens Analytics

**AI-powered investment research combining financial performance with strategic innovation signals**

Traditional investment analysis relies on financial metrics alone — stock growth, revenue, market cap. But numbers don't tell you whether a company is prepared for the future. DualLens Analytics solves this by combining quantitative financial data with qualitative insights extracted from strategy documents, giving investors a unified view of both financial strength and innovation readiness.

---

## Business Outcome

- Ranks companies by a dual signal: financial growth trajectory + AI initiative activity
- Eliminates manual cross-referencing of stock data and strategy PDFs
- Delivers structured, auditable investment rankings with source citations

---

## How It Works

1. **Financial data ingestion** — pulls 3-year stock performance from Yahoo Finance
2. **Document ingestion** — loads and chunks company strategy PDFs
3. **RAG pipeline** — embeds documents into a vector store for semantic retrieval
4. **Synthesis** — LLM combines financial scores with retrieved strategic insights
5. **Ranking output** — companies ranked by composite score with reasoning

---

## Architecture

```
Yahoo Finance API  ──┐
                     ├──► LLM Synthesis ──► Ranked Investment Report
Strategy PDFs ──► RAG (ChromaDB) ──┘
```

---

## Technologies

| Component | Technology |
|---|---|
| Orchestration | LangChain |
| Vector Store | ChromaDB |
| Embeddings | OpenAI |
| Financial Data | Yahoo Finance (yfinance) |
| Document Processing | PyPDF |
| LLM | OpenAI GPT-4o |

---

## Key Concepts Demonstrated

- Retrieval-Augmented Generation (RAG) for private document knowledge
- Hybrid ranking combining structured (numeric) and unstructured (semantic) signals
- Source-cited outputs to prevent hallucination and support audit trails

---

## Part of

[Agentic AI Architecture — Johns Hopkins University](https://github.com/kayvonsalari)
