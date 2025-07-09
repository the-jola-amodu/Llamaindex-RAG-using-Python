# 🧾 Intelligent Document Processing with RAG (PwC x Outamation Final Project)

This project is a **Retrieval-Augmented Generation (RAG) pipeline** built during an **externship with PwC**, hosted by **Outamation**. It is designed to **automate and optimize how banks and mortgage companies extract structured information** from unstructured documents (e.g., PDFs) submitted by clients.

By combining document classification, semantic chunking, vector search, and LLM reasoning, this solution offers a scalable foundation for document intelligence in regulated industries.

---

## 🧠 Key Capabilities

- 📄 **Accepts PDF documents** from customers (e.g., bank statements, pay stubs)
- 🧠 **Zero-shot classification** using **Facebook BART Large MNLI**
- ✂️ **Semantic chunking** of extracted text
- 🔍 **Hybrid Retrieval**:
  - Dense vector similarity (E5-base-v2 embeddings)
  - Keyword matching
- 💾 **LangChain Vector Store** integration
- 🧮 **LLM Switching Based on GPU Availability**:
  - 🔥 GPU Available: **Mistral 7B Instruct**
  - 🧊 No GPU: **TinyLlama 1.1B**
- 💬 Query-driven information retrieval using context + custom system prompt

---

## 🔧 Tech Stack

| Component                 | Tool/Library                         |
|---------------------------|--------------------------------------|
| **Language**              | Python                               |
| **PDF Processing**        | `pymupdf`                            |
| **Classification**        | `facebook/bart-large-mnli` (HuggingFace) |
| **Embedding Model**       | `intfloat/e5-base-v2`                |
| **Vector Store**          | LangChain                            |
| **Retrieval**             | Hybrid (Vector + Keyword)            |
| **LLMs**                  | Mistral 7B Instruct / TinyLlama 1.1B |
| **Execution Environment** | Google Colab (CUDA GPU)              |

---
## 🚀 How It Works

1. **Upload & Process PDF**  
   Uses `pymupdf` to extract text from multi-page PDFs.

2. **Classify Document Type**  
   - Zero-shot classification via **Facebook BART MNLI**  
   - Documents are tagged and stored based on type

3. **Chunk & Embed**  
   - Semantic chunking splits text at natural language boundaries  
   - Embeddings are generated using **E5-base-v2**

4. **Store in Vector DB**  
   - Text chunks and embeddings are stored in a **LangChain Vector Store**

5. **Query-Time Retrieval**  
   - A **hybrid retriever** uses both dense vector similarity and keyword matching  
   - Retrieves the most relevant document chunks for the query

6. **LLM Reasoning**  
   - System checks for **GPU availability** in the Google Colab environment  
     - ✅ If CUDA is available: use **Mistral 7B Instruct**  
     - ❌ If not: fallback to **TinyLlama 1.1B**  
   - Retrieved context + user query are passed to the chosen LLM to generate an informed response

### Prerequisites

Included in the project. Enjoy!!
