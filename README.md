# RAG Chatbot

A document-based chatbot built using Streamlit, FastAPI, and FAISS.  
It allows users to ask questions about PDFs and text files, retrieves relevant context using embeddings, and stores chat history in PostgreSQL.  

## How to Run
1. Install dependencies: `pip install -r requirements.txt`  
2. Run backend: `uvicorn backend/main:app --reload`  
3. Run frontend: `streamlit run frontend/app.py`  

> Demo video: `demo.mp4`
