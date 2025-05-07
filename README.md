# RAG-Demo

A simple Retrieval-Augmented Generation (RAG) system for document-based Q&A using [LangChain](https://python.langchain.com/), [ChromaDB](https://www.trychroma.com/), and [Streamlit](https://streamlit.io/).

---

## 🚀 Overview

This project demonstrates how to build a basic RAG pipeline:
- **Document chunking and retrieval**: Fetches and splits web documents into manageable chunks.
- **Vector storage**: Stores document embeddings in ChromaDB for efficient similarity search.
- **Answer generation**: Uses OpenAI's API to generate answers based on retrieved context.
- **Web interface**: Interact with the system via a simple Streamlit app.

---

## 🛠️ Features

- Load and process web documents
- Store and retrieve document embeddings with ChromaDB
- Interactive Q&A via Streamlit

---

## ⚡ Quickstart

### 1. Clone the repository

```bash
git clone https://github.com/ahmednoorx/RAG-Demo.git
cd RAG-Demo
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Set up your OpenAI API key

Create a `.env` file in the project root:

```
OPENAI_API_KEY=your_api_key_here
```

> **Note:** Never share your `.env` file or API keys publicly. The `.env` file is included in `.gitignore`.

### 4. Run the app

```bash
streamlit run app.py
```

---

## 📝 How it Works

1. **Document Loading**: Loads content from specified URLs using `UnstructuredURLLoader`.
2. **Chunking**: Splits documents into chunks for better retrieval.
3. **Embedding & Storage**: Embeds chunks and stores them in ChromaDB.
4. **Retrieval**: Finds relevant chunks using similarity search.
5. **Answer Generation**: Uses OpenAI's LLM to answer user queries based on retrieved context.
6. **Web UI**: Streamlit provides a chat-like interface for user interaction.

---

## 📚 What I Learned

- Implementing a basic RAG system with LangChain and ChromaDB
- Managing API keys securely with environment variables
- Building interactive apps with Streamlit

---

## 🙏 Acknowledgments

Based on a YouTube tutorial, with additional enhancements and modifications.

---
