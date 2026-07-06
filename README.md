
---

# 🧠 MCP Memory Agent — Knowledge Graph AI System

## 📌 Overview


**LINK-:** https://knowledge-graph-memory-mcp.vercel.app/

MCP Memory Agent is a full-stack **AI-powered memory and reasoning system** built using a multi-agent architecture. It goes beyond traditional chatbots by introducing a **structured knowledge graph memory layer** that allows persistent, semantic, and relationship-aware recall of information.

Unlike conventional chat applications that rely only on conversation history, this system extracts, stores, and retrieves memory in a structured format using AI agents, enabling long-term contextual excellence.
---

## 🚀 Live Architecture

```
Frontend (Next.js)  →  Backend (FastAPI)  →  Groq LLM + Memory System
        │                        │
        │                        ├── Agent Service (Orchestration)
        │                        ├── Memory Service (Graph Storage)
        │                        ├── Groq Service (LLM reasoning)
        │                        └── API Layer (Routes)
        │
        └── Vercel Deployment
Backend → Render Deployment
```

---

## ✨ Key Features

### 🧠 1. Knowledge Graph Memory System

* Converts user interactions into structured relationships
* Stores memory as entities + relationships instead of raw text
* Enables long-term contextual intelligence

---

### 🤖 2. Multi-Agent Architecture

The system is divided into specialized agents:

* **Agent Service** → Orchestrates workflow
* **Memory Service** → Stores and retrieves structured memory
* **Groq Service** → Handles LLM inference
* **API Layer** → Exposes endpoints for frontend communication

---

### ⚡ 3. Semantic Memory Retrieval

* Retrieves context based on meaning, not just chat history
* Works even after long time gaps
* Improves personalization and continuity

---

### 🌐 4. Full-Stack Deployment

* Frontend deployed on **Vercel**
* Backend deployed on **Render**
* Production-ready environment with CORS handling

---

### 🎨 5. Modern UI

* Built with **Next.js 16 (App Router)**
* Responsive and minimal UI
* Real-time chat interaction

---

## 🛠️ Tech Stack

### Frontend

* Next.js 16
* React 19
* Tailwind CSS
* Axios
* Lucide Icons

### Backend

* FastAPI
* Python 3.10+
* Pydantic
* Uvicorn

### AI / LLM

* Groq API (LLaMA models)
* Agent-based reasoning pipeline

### Deployment

* Vercel (Frontend)
* Render (Backend)

---

## 📁 Project Structure

```
knowledge-graph-memory-mcp/
│
├── frontend/                 # Next.js frontend
│   ├── src/app/
│   ├── src/lib/api.ts
│   ├── public/
│   └── package.json
│
├── backend/                 # FastAPI backend
│   ├── app/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── utils/
│   │   ├── models/
│   │   └── config.py
│   └── requirements.txt
│
├── mcp_newer.ipynb         # Experimentation notebook
└── README.md
```

---

## 🔌 API Endpoints

### Health Check

```
GET /
```

### Chat Endpoint

```
POST /chat
```

#### Request

```json
{
  "message": "Hello"
}
```

#### Response

```json
{
  "response": "AI generated reply"
}
```

---

## ⚙️ How It Works

1. User sends a message from frontend
2. Backend receives request via FastAPI
3. Agent Service processes input
4. Memory Service stores structured knowledge
5. Groq LLM generates intelligent response
6. Response is returned to frontend
7. Memory is updated for future context

---

## 🧠 Why This Project is Different

Unlike traditional chatbots:

| Feature      | ChatGPT-style Chatbot | MCP Memory Agent        |
| ------------ | --------------------- | ----------------------- |
| Memory Type  | Chat history          | Knowledge graph         |
| Retrieval    | Last messages         | Semantic search         |
| Structure    | Unstructured text     | Entities + relations    |
| Intelligence | Context window        | Persistent reasoning    |
| Scalability  | Limited               | Extensible agent system |

---

## 🚀 Deployment

### Frontend (Vercel)

* Set root directory: `frontend`
* Build command: `npm run build`
* Output: `.next`
* Env:

```
NEXT_PUBLIC_API_URL = <backend-url>
```

---

### Backend (Render)

* Python FastAPI service
* Start command:

```
uvicorn app.main:app --host 0.0.0.0 --port 10000
```

---

## 🧩 Challenges Solved

* CORS issues between frontend and backend
* Production deployment mismatches
* API route alignment
* Environment variable configuration
* Next.js App Router deployment structure

---

## 📌 Future Improvements

* Persistent vector database (Chroma / Pinecone)
* Advanced graph visualization
* User-specific memory isolation
* Authentication layer
* Streaming responses (real-time AI chat)

---

## 👨‍💻 Author

**Prateek Choudhary**
AI/ML & Full Stack Developer
Focus: Agentic AI systems, RAG pipelines, scalable backend architectures

---

## ⭐ If you like this project

Give it a star ⭐ and share it with others interested in:

* AI Agents
* Memory Systems
* LLM Applications
* Full Stack AI Engineering

---
