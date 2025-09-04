# 🤖 RAG Chatbot with FAISS and LLaMA

A **Retrieval-Augmented Generation (RAG)** chatbot that allows you to upload PDFs and ask questions about their content.  
It uses **LangChain, HuggingFace embeddings, FAISS vector database, and Ollama’s LLaMA model** to build a local AI-powered knowledge assistant with an easy-to-use **Streamlit** interface.

---

## 🧠 How RAG Works

---

**Retrieval-Augmented Generation (RAG)** is a technique that improves large language models (LLMs) by combining them with external knowledge sources.
## ✨ Features
- 📄 Upload **PDF documents** and extract their text
- 🧩 Split documents into chunks for better context handling
- 🔎 Store & retrieve text using **FAISS** vector database
- 🧠 Answer questions with **LLaMA (via Ollama)**
- 🌐 Simple & interactive **Streamlit UI**
- ⚡ Runs **locally** — no external API calls needed

---


Here’s how this project implements RAG:

**Step-by-step workflow:**
1. **Extract PDF Text** → Convert uploaded PDF into raw text.  
2. **Chunking** → Split text into manageable chunks.  
3. **Embeddings** → Encode chunks using HuggingFace models.  
4. **Store in FAISS** → Save embeddings in a vector database for similarity search.  
5. **Retrieve** → Fetch the most relevant chunks for a query.  
6. **Generate Answer** → LLaMA uses the retrieved context to generate accurate responses.

This ensures the chatbot **grounds its answers in the actual document**, rather than hallucinating.
