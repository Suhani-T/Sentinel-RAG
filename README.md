# Sentinel-RAG

A production-inspired Retrieval-Augmented Generation (RAG) knowledge base that enables users to upload and query complex documents with accurate, explainable, and evaluated responses.

The project progressively evolves from a basic RAG pipeline into an advanced document intelligence system featuring source attribution, retrieval optimization, reranking, guardrails, automated evaluation, and observability.

---

## Problem Statement

Large documents such as:

- Financial Reports
- Research Papers
- API Documentation
- Company Policies
- Medical Records

contain valuable information that is difficult to search manually.

Traditional LLMs cannot reliably answer questions about these documents and may hallucinate information.

SentinelRAG addresses this by retrieving relevant context from uploaded documents and grounding responses in verified source material.

---

## Tech Stack

| Component | Technology |
|------------|------------|
| Backend | FastAPI |
| Frontend | Streamlit |
| Language | Python |
| LLM | Gemini 2.5 Flash |
| Embeddings | all-MiniLM-L6-v2 |
| Vector Database | ChromaDB |
| PDF Parsing | PyMuPDF |
| Chunking | RecursiveCharacterTextSplitter |
| Advanced Retrieval | Parent-Child Retrieval, Sentence Window Retrieval |
| Reranking | BGE-Reranker |
| Evaluation | RAGAS |
| Guardrails | Custom Validation Pipeline |
| Logging | SQLite |

---

## Features

### Document Ingestion

- Upload one or multiple PDFs
- Automatic text extraction
- Chunk creation and embedding generation
- Metadata preservation

### Semantic Search

- Vector similarity search using ChromaDB
- Context-aware retrieval
- Multi-document querying

### Source Attribution

- PDF source tracking
- Page-level citations
- Explainable responses

### Advanced Retrieval

- Parent-Child Retrieval
- Sentence Window Retrieval
- Retrieval strategy comparison

### Reranking

- BGE-Reranker integration
- Improved context relevance
- Reduced retrieval noise

### Guardrails

- Prompt injection detection
- Output validation
- Sensitive information filtering
- Hallucination reduction

### Evaluation

- RAGAS-based benchmarking
- Faithfulness measurement
- Context Recall measurement
- Context Precision measurement
- Answer Relevancy measurement

---

### Assessment Loop

- Response verification
- Context grounding checks
- Retry and refusal mechanisms

### Observability

- Query logging
- Retrieval logging
- Reranker score tracking
- Latency monitoring
  
---

## Evaluation Metrics

The project focuses on measurable retrieval quality rather than subjective performance.

Metrics include:

- Faithfulness
- Context Recall
- Context Precision
- Answer Relevancy
- Latency
- Retrieval Accuracy

---
