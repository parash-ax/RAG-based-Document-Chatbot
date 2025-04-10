# 🧠 RAG-Based Document Chatbot

A **Retrieval-Augmented Generation (RAG)** powered chatbot that answers user queries from long documents (PDFs, text, etc.) with high accuracy, minimal hallucination, and fast response time.

![Chatbot Banner](https://media.giphy.com/media/3oEjI6SIIHBdRxXI40/giphy.gif)

---

## 🚀 Features

- 🔍 **Context-Aware Retrieval** using FAISS vector database
- 🤖 **Open-Source LLMs** (e.g., Gemma, Mistral) via Hugging Face or Ollama
- 🔄 **Hybrid Retrieval**: Dense (Embeddings) + Sparse (BM25)
- 📄 Supports **PDF/Text** documents
- 🕒 **Low Latency** (<1.5s) using GPU (Google Colab compatible)
- 🗂️ **Structured Output**: Paragraphs, bullet points, tables
- 💬 Handles **follow-up questions** and conversational context
- 🌐 **Streamlit Web UI** for a clean, user-friendly experience

---

## 📸 Demo

![Chatbot UI Demo](https://user-images.githubusercontent.com/yourusername/your-demo-image.png)

> 👆 Replace with your actual screenshot or recording

---

## 🛠️ Tech Stack

- `Python 3.10+`
- `FAISS` for vector search
- `Hugging Face Transformers` (Gemma / Mistral models)
- `Sentence Transformers` or `BGE Embeddings`
- `BM25` (via `rank_bm25` or `Whoosh`)
- `Streamlit` for UI
- `PyMuPDF / pdfplumber` for PDF reading
- `Google Colab` / `Kaggle` GPU (for inference)

---

## ⚙️ How to Run Locally

```bash
# 1. Clone the repo
git clone https://github.com/yourusername/rag-document-chatbot.git
cd rag-document-chatbot

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the app
streamlit run app.py
