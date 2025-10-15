

# 🔍 RAG Knowledge Base Search Engine

AI-powered document search system using *Retrieval-Augmented Generation (RAG)* and *Google Gemini API*.

## 📋 Features

- 📄 Upload PDF and TXT documents
- 🤖 Ask questions in natural language
- 💡 Get AI-generated answers with source citations
- 🎨 Clean, modern web interface
- ⚡ Fast semantic search using embeddings

## 🛠 Tech Stack

- *Backend*: Flask (Python)
- *Embeddings*: Sentence-Transformers (all-MiniLM-L6-v2)
- *LLM*: Google Gemini Pro API
- *Vector Search*: NumPy (Cosine Similarity)
- *Frontend*: HTML5, CSS3, Vanilla JavaScript

## 🚀 How It Works (RAG Pipeline)

1. *Document Upload*: PDF/TXT files are uploaded
2. *Text Extraction*: PyPDF2 extracts text from documents
3. *Chunking*: Documents split into 500-character chunks
4. *Embedding*: Each chunk converted to 384-dim vector using Sentence-Transformers
5. *Storage*: Embeddings stored in NumPy array (in-memory)
6. *Query Processing*: User question converted to embedding
7. *Retrieval*: Top-3 most similar chunks found using cosine similarity
8. *Generation*: Gemini AI synthesizes answer from retrieved chunks

## Demo Video
<video src="video5759624597.mp4" controls width="600"></video>

## 📦 Installation

### Prerequisites
- Python 3.8+
- Gemini API Key (get free at https://ai.google.dev)

### Setup

1. *Clone the repository*
bash
git clone https://github.com/YOUR-USERNAME/rag-knowledge-search.git
cd rag-knowledge-search


2. *Create virtual environment*
bash
python -m venv venv


3. *Activate virtual environment*
- Windows:
bash
  venv\Scripts\activate

- Mac/Linux:
bash
  source venv/bin/activate


4. *Install dependencies*
bash
pip install flask PyPDF2 sentence-transformers google-generativeai numpy


5. *Add your Gemini API Key*
- Open app.py
- Replace YOUR_GEMINI_API_KEY_HERE with your actual API key

6. *Run the application*
bash
python app.py


7. *Open in browser*

