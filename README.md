# 📄 PDF-RAG: Local Question Answering Over PDFs

This project is a **local Retrieval-Augmented Generation (RAG) application** that allows users to upload a PDF file and ask questions about its content. It uses **LangChain**, **Streamlit**, **Chroma vector database**, **HuggingFace embeddings**, and **Ollama** for running large language models locally.

---

## 🚀 Features

- 📂 Upload any PDF file via a simple web interface  
- ✂️ Automatically splits PDF text into chunks  
- 🧠 Generates embeddings using HuggingFace models  
- 🗄️ Stores embeddings locally using Chroma  
- 🤖 Uses Ollama to run LLMs **fully locally**  
- 🔍 Retrieves relevant PDF sections to answer questions  
- 📌 Displays source pages for transparency  

---

## 🏗️ Architecture Overview

1. **PDF Upload (Streamlit Sidebar)**
2. **Document Loading** using `PyPDFLoader`
3. **Text Chunking** with `RecursiveCharacterTextSplitter`
4. **Embedding Generation** via HuggingFace
5. **Vector Storage** using Chroma
6. **Question Answering** with LangChain `RetrievalQA`
7. **LLM Inference** using Ollama (e.g., `llama3.2`)

---

## 🛠️ Tech Stack

- **Frontend**: Streamlit  
- **LLM Framework**: LangChain  
- **Vector Database**: Chroma  
- **Embeddings**: HuggingFace Embeddings  
- **LLM Runtime**: Ollama  
- **Language**: Python  

---

## 📦 Installation

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/aniragn/RAG_App.git
cd RAG_App