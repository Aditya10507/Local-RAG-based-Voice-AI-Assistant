# Personal AI Assistant (Local RAG + Voice)

## Overview

A fully local **AI-powered personal assistant** built using a Retrieval-Augmented Generation (RAG) pipeline. The system can understand documents, answer questions contextually, and interact through **voice input and output** — all without relying on paid APIs.

---

##  Features

**Document Understanding**
  Extracts and processes PDFs using chunking and embeddings.

**RAG Pipeline**
  Combines semantic search (FAISS) with LLM reasoning for accurate answers.

**Conversational Memory**
  Maintains chat history for multi-turn interactions.

**Voice Assistant**

  * Speech-to-Text using Whisper
  * Text-to-Speech using pyttsx3

  **Fully Local Setup**
  Runs entirely offline using Ollama + Mistral (no API cost).

---

##Tech Stack

* **Language:** Python
* **LLM:** Mistral (via Ollama)
* **Embeddings:** Sentence Transformers
* **Vector DB:** FAISS
* **Speech-to-Text:** Whisper
* **Text-to-Speech:** pyttsx3

---

##Project Structure

```
rag-assistant/
│
├── ingest.py        # PDF processing + embedding generation
├── query.py         # RAG pipeline + response generation
├── voice.py         # Voice input/output integration
├── README.md
├── requirements.txt
└── .gitignore
```

---

##Setup Instructions

### 1. Clone the repository

```
git clone https://github.com/Aditya10507/Local-RAG-based-Voice-AI-Assistant.git
cd rag-assistant
```

### 2. Create virtual environment

```
python -m venv venv
venv\Scripts\activate   # Windows
```

### 3. Install dependencies

```
pip install -r requirements.txt
```

### 4. Start Ollama (for Mistral)

```
ollama run mistral
```

### 5. Run the assistant

```
python query.py
```

---

##Use Cases

* Personal knowledge assistant
* Resume/document Q&A system
* Offline AI chatbot
* Voice-enabled AI applications

---

##Key Learnings

* Built a complete **RAG architecture from scratch**
* Implemented **semantic search using FAISS**
* Integrated **LLMs locally without APIs**
* Developed **voice-enabled AI interactions**
* Managed **clean Git workflows and project structure**

---

##Future Improvements

* Web interface (Streamlit / React)
* Multi-document support
* Real-time voice assistant
* Deployment as a desktop app

---

##Author

**Aditya Singh**
Aspiring AI/ML Engineer focused on building real-world intelligent systems.

---

##If you like this project

Give it a ⭐ on GitHub and feel free to contribute!
