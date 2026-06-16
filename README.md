NyaySetu — AI-Powered Legal Assistance Platform
NyaySetu is an AI-powered legal assistance platform designed to simplify legal information and improve accessibility to legal guidance. It leverages Large Language Models (LLMs), Retrieval-Augmented Generation (RAG), semantic search, and predictive analytics to help users understand legal procedures, analyze documents, and explore similar legal cases.

Features
1. AI Legal Assistant Chatbot (RAG Pipeline)
* Built an intelligent legal chatbot using a **Retrieval-Augmented Generation (RAG)** pipeline.
* Retrieves relevant legal context and generates simplified legal guidance for users.
* Powered by **LLaMA 3 via Ollama** for locally hosted inference.

2. Case Outcome Prediction
Predicts the likelihood of favorable legal outcomes based on:
  * State
  * Court Type
  * Case Type
  * Number of Hearings
  * Complexity of the Case
  Helps users gain data-driven legal insights.

3. PDF Legal Document Analyzer
Upload legal PDF documents for:

  * Information extraction
  * Summarization
  * Legal content understanding
  Uses parallel LLaMA models for extraction and summarization.
  Includes a judge model for response validation.
  Deployed locally using Ollama and exposed through ngrok.

4. Similar Cases Retrieval
* AI-powered legal case recommendation system.
* Refines user queries using LLMs.
* Retrieves legal judgments through the **Indian Kanoon API**.
* Uses **FAISS vector search** and embeddings for semantic similarity matching.
* Re-ranks relevant legal cases and generates concise AI summaries.

Tech Stack
Backend
* Python
* FastAPI

AI/ML
* LLaMA 3 (via Ollama)
* SentenceTransformers
* FAISS
* RAG Pipeline

Data Processing
* pdfplumber
* Pandas

Frontend
* React.js

Tools
* Git
* ngrok
* Ollama

System Architecture
1. User submits a legal query/document
2. Query is refined using LLMs
3. Relevant legal context is retrieved
4. FAISS semantic similarity search is performed
5. LLaMA generates simplified legal insights
6. Results are summarized and displayed to users

Key Highlights
* Local LLM deployment using Ollama
* RAG-based legal retrieval system
* Semantic legal case similarity search using **FAISS**
* AI-powered legal document analysis
* Case outcome prediction engine

Installation
Clone the repository:


git clone https://github.com/your-username/NyaySetu.git
cd NyaySetu

Install dependencies:

pip install -r requirements.txt

Run the backend:

uvicorn main:app --reload


Run the frontend:


npm install
npm start

Future Improvements

* Multi-language legal assistance
* Voice-enabled legal chatbot
* Improved legal case prediction models
* Cloud deployment support

License
This project is intended for educational and research purposes.
