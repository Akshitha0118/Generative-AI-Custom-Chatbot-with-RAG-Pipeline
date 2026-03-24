# 🚀Generative-AI-Custom-Chatbot-with-RAG-Pipeline

Turn any PDF into an intelligent AI-powered Q&A system using Retrieval-Augmented Generation (RAG).

---

## 📌 Overview

This project implements a **Retrieval-Augmented Generation (RAG)** pipeline that allows users to ask questions from a PDF document and receive **context-aware, accurate answers along with source references**.

Instead of relying solely on LLM knowledge, this system retrieves relevant chunks from the document and feeds them into the model — ensuring **grounded and reliable responses**.

---

## ✨ Features

- 📄 Load PDF directly from a URL
- 🔍 Intelligent text chunking for better retrieval
- 🧠 Semantic search using embeddings
- 🗂️ Vector storage using ChromaDB
- ⚡ Fast inference using Groq LLM
- 🔗 RetrievalQA pipeline with LangChain
- 📌 Returns answers **with source context**
- 💡 Scalable and modular design

---

## 🛠️ Tech Stack

- **Python**
- **LangChain**
- **ChromaDB (Vector Database)**
- **HuggingFace Embeddings**
- **Groq API (LLM - LLaMA 3)**
- **Unstructured (PDF Loader)**

---

## 🏗️ Architecture

            
            │   PDF Document     │
            
                     │
                     ▼
      
      │ Unstructured File Loader    │
      
               │
               ▼
    
    │ Text Chunking (Splitter)   │

             │
             ▼

 │ HuggingFace Embeddings     │

          │
          ▼
 
 │ Chroma Vector Database     │

          │
          ▼
   
     │ Retriever       │
   
               │
               ▼

     │ Groq LLM (LLaMA 3)    │
    
          │
          ▼
          
  ✅ Final Answer + Sources
    
