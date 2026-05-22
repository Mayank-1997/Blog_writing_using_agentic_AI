# AI Blog Writer Agent

An advanced **Agentic AI-powered Blog Generation System** built using **LangGraph**, **LangChain**, **FastAPI**, **Streamlit**, **OpenAI GPT-4.1**, **Tavily Search**, and **Gemini Image Generation**.

This project demonstrates how multiple AI agents can collaboratively research, plan, write, and enrich high-quality technical blogs automatically using modern Agentic AI architecture.

---

# 🚀 Project Vision

The goal of this system is to build a fully autonomous **AI Blog Writing Agent** capable of:

- Understanding a user topic
- Deciding whether internet research is needed
- Performing real-time web research
- Planning the blog structure intelligently
- Parallel content generation using worker agents
- Adding citations and references
- Generating technical diagrams/images automatically
- Producing final markdown blog output
- Rendering blogs in a frontend application
- Exporting blogs as PDF/DOCX

This project showcases practical implementation of:

- Agentic AI
- Multi-agent orchestration
- LLM workflows
- Parallel execution
- AI research systems
- AI content pipelines

---

# 🧠 Agentic Workflow Architecture

```text
User Topic
    ↓
Router Agent
    ↓
(Research Needed?)
    ↓
Research Agent (Tavily)
    ↓
Orchestrator Agent
    ↓
Parallel Worker Agents
    ↓
Reducer Agent
    ↓
Image Planning Agent
    ↓
Gemini Image Generation
    ↓
Final Blog Output
```

---

# ⚙️ Core Features

## ✅ Intelligent Research Routing

The Router Agent decides:
- Whether web research is needed
- Which research mode to use:
  - `closed_book`
  - `hybrid`
  - `open_book`

---

## ✅ Real-Time Web Research

Integrated with:
- Tavily Search API

The system gathers:
- latest AI news
- framework updates
- citations
- technical references

---

## ✅ Multi-Agent Blog Planning

The Orchestrator Agent:
- creates complete blog outlines
- defines sections
- generates goals
- assigns writing tasks

---

## ✅ Parallel Worker Agents

Each worker agent:
- independently generates one section
- follows constraints
- cites evidence
- adds code snippets when needed

---

## ✅ AI Image & Diagram Generation

Integrated with:
- Google Gemini 2.5 Flash Image

The system automatically:
- detects where diagrams are useful
- inserts image placeholders
- generates technical diagrams
- embeds images into markdown

---

## ✅ Streamlit Frontend

Frontend capabilities:
- Topic prompt input
- Blog rendering
- Session blog history
- Markdown rendering

---

# 🏗️ Tech Stack

## AI / LLM Stack

| Technology | Purpose |
|---|---|
| GPT-4.1 Mini | Blog generation |
| LangGraph | Agent orchestration |
| LangChain | LLM integrations |
| Tavily Search | Web research |
| Gemini 2.5 Flash Image | AI image generation |

---

## Backend Stack

| Technology | Purpose |
|---|---|
| FastAPI | API layer |
| Pydantic | Schema validation |
| Python | Core backend |

---

## Frontend Stack

| Technology | Purpose |
|---|---|
| Streamlit | Frontend UI |
| ReactMarkdown | Markdown rendering |

---

# 📂 Project Structure

```bash
project/
│
├── bwa_backend.py
├── bwa_frontend.py
├── requirements.txt
├── .env.example
├── README.md

```

---

# 🌐 API Endpoints


```

## Generate Blog

```http
POST /api/generate
```

### Request

```json
{
  "topic": "LangGraph Multi Agent Systems"
}
```

### Response

```json
{
  "topic": "LangGraph Multi Agent Systems",
  "title": "Building Multi-Agent Systems with LangGraph",
  "markdown": "# Blog Content...",
  "generated_at": "2026-05-22"
}
```

---

# 🖥️ Local Setup

## 1. Clone Repository

```bash
git clone <repo_url>
cd project
```

## 2. Create Virtual Environment

```bash
python -m venv venv
```

### Activate (Windows)

```bash
venv\Scripts\activate
```

### Activate (Linux/Mac)

```bash
source venv/bin/activate
```

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

## 4. Configure Environment Variables

Create `.env`

```env
OPENAI_API_KEY=your_key
TAVILY_API_KEY=your_key
GOOGLE_API_KEY=your_key
```

## 5. Run Application

```

### Streamlit Frontend

```bash
streamlit run bwa_frontend.py
```

---

# 🎯 Use Cases

- Technical blogging
- AI news summarization
- Developer advocacy
- AI content generation
- Research automation
- Knowledge synthesis
- Educational content generation

---

# 🔥 Highlights of This Project

✅ Multi-Agent Systems  
✅ Parallel AI Workflows  
✅ AI Planning Systems  
✅ AI Research Pipelines  
✅ Retrieval-Augmented Generation (RAG)  
✅ Structured LLM Outputs  
✅ Graph-based Agent Orchestration  
✅ AI Tool Usage  
✅ Autonomous Content Pipelines  

---

# 📈 Future Enhancements

Potential future upgrades:

- Streaming responses
- Persistent database storage
- Authentication
- Blog editing
- Multi-language generation
- SEO optimization
- One-click Medium publishing
- WebSocket progress updates
- Human-in-the-loop review
- AI memory systems

---

# 👨‍💻 Author

Built as an advanced Agentic AI engineering project demonstrating practical usage of:

- LangGraph
- LangChain
- OpenAI APIs
- Tavily
- Gemini
- FastAPI
- Streamlit

for real-world autonomous AI systems.

---

# 📜 License

MIT License
