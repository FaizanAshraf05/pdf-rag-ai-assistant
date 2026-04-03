# Local RAG AI Assistant (Chat with PDF)

## 📌 Project Overview
This project is a fully functional Retrieval-Augmented Generation (RAG) pipeline. It allows users to upload complex, proprietary PDF documents and "chat" with them using a Large Language Model. The system ensures AI responses are strictly grounded in the provided document, eliminating hallucinations.

## 🚀 The AI Architecture
* **Document Ingestion:** Utilizes `PyPDF` and LangChain's `RecursiveCharacterTextSplitter` to parse and chunk large documents for optimized semantic search.
* **Vector Database:** Converts text chunks into high-dimensional embeddings using Hugging Face's `all-MiniLM-L6-v2` model, storing them locally in a `FAISS` database.
* **LLM Integration:** Connects the FAISS retriever to Google's `Gemini 2.5 Flash` API via LangChain, generating highly accurate, context-aware answers.
* **Security:** Implements environment variables (`.env`) for secure API key management.

## 🛠️ Tech Stack
* **Python**
* **LangChain** (Orchestration)
* **FAISS** (Vector Database)
* **Google Gemini API** (LLM)
* **Hugging Face** (Embeddings)

---
*Developed to demonstrate advanced RAG architecture, vector database implementation, and secure API integration.*
