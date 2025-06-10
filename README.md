# 💬 Real-time LLM Chat App

A real-time chat interface powered by **Streamlit**, **FastAPI**, **Socket.IO**, and **Ollama (or OpenAI-compatible LLMs)**. It allows multiple users to interact with an LLM backend seamlessly through a browser-based UI.

---

## ⚙️ Tech Stack

- **Frontend:** Streamlit + Python Socket.IO Client  
- **Backend:** FastAPI + Python Socket.IO Server  
- **LLM Engine:** Local LLM via [Ollama](https://ollama.com/) or OpenAI-compatible APIs  
- **Containerization:** Docker + Docker Compose

---

## 📁 Project Structure

```
realtime-llm-chat-app/
├── backend/                 # FastAPI backend with LLM and Socket.IO
│   ├── app.py
│   ├── requirements.txt
├── frontend/                # Streamlit frontend UI with real-time chat
│   ├── streamlit_app.py
│   ├── requirements.txt
├── docker-compose.yml       # Compose file to run frontend & backend
├── Dockerfile.backend       # Backend Dockerfile
├── Dockerfile.frontend      # Frontend Dockerfile
└── README.md
```

---

## 🚀 Getting Started

### 🛠️ Prerequisites

- Docker and Docker Compose installed  
- [Ollama](https://ollama.com/download) installed (for local LLMs) — optional if using OpenAI

---

### 🐳 Run with Docker

```bash
docker compose build
docker compose up
```

- Access frontend: [http://localhost:8501](http://localhost:8501)  
- Backend API: [http://localhost:8000](http://localhost:8000)

---

## 🔌 How It Works

- Frontend connects to backend via **Socket.IO**
- Messages are sent in real-time to the FastAPI backend
- Backend queries an LLM (Ollama or OpenAI) and returns responses
- All services are containerized and run together via Docker Compose

---

## ✅ Features

- Real-time WebSocket chat interface  
- Supports multiple clients simultaneously  
- Pluggable LLM backend (Ollama/OpenAI/etc.)  
- Clean UI built with Streamlit  
- Cross-platform, Dockerized setup

---

## 🧠 Future Improvements

- Add authentication / user sessions  
- Store chat history using a database  
- Improve error handling and reconnects  
- Support advanced LLM parameters (temperature, max tokens, etc.)

---

## 🙋‍♂️ Author

**Akshay Mehta**  
🔗 [GitHub Profile](https://github.com/Mrakshaymehta)

---

## 📝 License

MIT License – free to use and modify
