# 📚 CourseMateAI - RAG Based PDF Question Answering System

CourseMateAI is a Retrieval-Augmented Generation (RAG) application that allows users to upload PDF documents and ask questions about their content. The system retrieves the most relevant information from the uploaded document using vector embeddings and generates accurate responses using Mistral AI.

---

## 🚀 Live Demo

🔗 **Live Application:** https://sentence-completio-npkqxziprzaewgbz8fz24r.streamlit.app/

---

## ✨ Features

- Upload PDF documents
- Automatically split documents into chunks
- Generate embeddings using **BAAI/bge-small-en-v1.5**
- Store embeddings in **ChromaDB**
- Retrieve relevant document chunks using **MMR Retrieval**
- Generate answers using **Mistral AI**
- Interactive Streamlit interface

---

## 🛠️ Tech Stack

- Python
- Streamlit
- LangChain
- Mistral AI
- Hugging Face Embeddings
- ChromaDB
- PyPDF
- Sentence Transformers

---

## 📂 Project Structure

```
CourseMateAI/
│
├── app.py
├── create_database.py
├── chroma_db/
├── requirements.txt
├── .env
└── README.md
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone <your-repository-url>
```

```bash
cd CourseMateAI
```

### Create Virtual Environment

```bash
python -m venv .venv
```

### Activate Environment

#### Windows

```bash
.venv\Scripts\activate
```

#### Linux / macOS

```bash
source .venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the project root.

```env
MISTRAL_API_KEY=YOUR_MISTRAL_API_KEY
```

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

---

## 📖 How It Works

1. Upload a PDF document.
2. The document is loaded using PyPDFLoader.
3. The document is split into smaller chunks.
4. Each chunk is converted into embeddings using **BAAI/bge-small-en-v1.5**.
5. Embeddings are stored in **ChromaDB**.
6. User enters a question.
7. The retriever fetches the most relevant chunks.
8. Mistral AI generates an answer using only the retrieved context.

---

## 🧠 Embedding Model

- **BAAI/bge-small-en-v1.5**

---

## 🤖 Language Model

- **Mistral Small Latest**

---

## 📚 Vector Database

- ChromaDB

---

## 🔍 Retrieval Strategy

- Maximum Marginal Relevance (MMR)

Configuration:

```python
search_type="mmr"

k=4
fetch_k=10
lambda_mult=0.5
```

---

## 📦 Dependencies

- LangChain
- LangChain Chroma
- LangChain HuggingFace
- LangChain MistralAI
- ChromaDB
- Sentence Transformers
- Streamlit
- PyPDF
- Python Dotenv

---

## 📸 Application Workflow

```
Upload PDF
      │
      ▼
Load Document
      │
      ▼
Split into Chunks
      │
      ▼
Generate Embeddings
      │
      ▼
Store in ChromaDB
      │
      ▼
User Question
      │
      ▼
Retrieve Relevant Chunks
      │
      ▼
Mistral AI
      │
      ▼
Answer
```

---

## 👨‍💻 Author

**Kakul Barsaiya**

B.Tech Computer Science Engineering

Manipal University Jaipur

---

## ⭐ If you like this project

Please consider giving this repository a ⭐ on GitHub.
