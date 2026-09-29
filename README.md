# 🎓 College AI Assistant

An AI-powered college chatbot that helps students get answers from college documents such as academic regulations, exam information, and other institutional resources.

The system uses **Retrieval-Augmented Generation (RAG)** to search relevant document content and generate answers using a local AI model.

## ✨ Features

* 🤖 AI-powered student chatbot
* 📄 Upload PDF, DOCX, and TXT documents
* 🔍 Semantic document search using ChromaDB
* 🧠 Local AI using Ollama
* 📚 Answers based on uploaded college documents
* 🔐 Student and Admin authentication
* 👨‍💼 Admin document management
* 📊 Admin analytics
* 📝 Source citations for answers
* 💾 Local SQLite database
* ⚡ React + FastAPI full-stack application

## 🛠️ Tech Stack

**Frontend**

* React
* Vite
* Tailwind CSS
* React Router
* Axios
* Recharts

**Backend**

* Python
* FastAPI
* SQLAlchemy
* JWT Authentication

**AI / RAG**

* Ollama
* Llama 3.2
* Sentence Transformers
* ChromaDB

**Document Processing**

* PyMuPDF
* python-docx

**Database**

* SQLite
* ChromaDB

## 🔄 How It Works

```text
College Documents
       ↓
Text Extraction
       ↓
Text Chunking
       ↓
Embeddings
       ↓
ChromaDB
       ↓
Relevant Information
       ↓
Ollama LLM
       ↓
AI Answer + Citations
       ↓
Student Chat Interface
```

## 📁 Project Structure

```text
college-ai-assistant/
├── backend/
│   ├── app/
│   │   ├── api/
│   │   ├── models/
│   │   ├── services/
│   │   └── utils/
│   ├── tests/
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   │   ├── pages/
│   │   ├── layouts/
│   │   ├── context/
│   │   └── services/
│   └── package.json
│
└── README.md
```

## 🚀 Setup

### Backend

```bash
cd backend
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

Create `.env` from `.env.example`.

### Frontend

```bash
cd frontend
npm install
```

### Ollama

Install Ollama and download the model:

```bash
ollama pull llama3.2
ollama serve
```

### Run Backend

```bash
cd backend
.venv\Scripts\activate
uvicorn app.main:app --reload --port 8000
```

### Run Frontend

```bash
cd frontend
npm run dev
```

Open:

```text
http://localhost:5173
```

API documentation:

```text
http://localhost:8000/docs
```

## 👤 Default Admin

```text
Email: admin@college.edu
Password: admin123
```

Change the default password after first login.

## 🎯 Use Cases

* College information chatbot
* Student academic assistance
* Exam and attendance queries
* College document search
* Institutional knowledge management
* AI-based student support

## 🔮 Future Improvements

* Voice-based interaction
* Multilingual support
* Mobile application
* More advanced analytics
* Cloud deployment
* Improved citation and document management

## 📌 Project

**College AI Assistant — RAG-Based Intelligent Student Support System**
