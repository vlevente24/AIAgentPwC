# Agentic RAG Chatbot Prototype

A LangGraph-based RAG chatbot prototype demonstrating autonomous tool-calling and decision-making. The agent dynamically chooses between local document retrieval, web search, or checking the system time to answer user queries.

## 🚀 Tech Stack
* **Framework:** LangGraph & LangChain
* **Vector DB:** ChromaDB (Local)
* **LLM Engine:** Ollama
* **Models:** `minimax-m2.5:cloud` (Core LLM), `nomic-embed-text` (Embeddings)

## 🛠️ Quick Setup

1. **Install Prerequisites:** Python 3.8+ and [Ollama](https://ollama.com/).
2. **Pull Local Models:**
   ```bash
   ollama pull nomic-embed-text
   ollama pull minimax-m2.5:cloud
   
3. **Install Python Dependencies:**
   ```bash
   uv add langgraph langchain ollama notebook langchain-ollama langchain-chroma langchain-community httpx pydantic ddgs pypdf 