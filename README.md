# RAG Chatbot

This is a Retrieval-Augmented Generation (RAG) Chatbot built using Streamlit for the frontend, FastAPI for the backend, and FAISS for semantic search. The project is created for learning how to build a full-stack RAG application using local embeddings.

Features
- Ask questions about documents (PDFs and text files)
- Context-aware answers using embeddings and vector search
- Interactive Streamlit frontend
- Backend with FastAPI and PostgreSQL to store users and chat history

Installation
1. Clone the repository:
git clone https://github.com/yourusername/RAG_chatbot.git
cd RAG_chatbot

2. Create and activate a virtual environment:
python -m venv venv
# Windows
venv\Scripts\activate
# Mac/Linux
source venv/bin/activate

3. Install dependencies:
pip install -r requirements.txt

4. Set up environment variables by creating a .env file with the following:
DATABASE_URL=your_postgresql_url
GOOGLE_API_KEY=your_google_api_key_if_used

5. Create FAISS embeddings by running:
python backend/create_index.py

6. Create database tables by running:
python backend/create_tables.py

7. Run the backend API:
cd backend
uvicorn main:app --reload

8. Run the frontend Streamlit app:
cd frontend
streamlit run app.py

Demo
You can watch a 30-second demo of the chatbot in the demo.mp4 file included in this repository.

Project Structure
RAG_chatbot/
├── backend/
│   ├── main.py
│   ├── create_index.py
│   └── create_tables.py
├── frontend/
│   └── app.py
├── faiss_index/
│   ├── index.faiss
│   └── index.pkl
├── knowledge_base/
│   ├── oops_java.pdf
│   └── webscraping.txt
├── demo.mp4
└── requirements.txt

Technologies Used
- Python
- Streamlit
- FastAPI
- FAISS
- PostgreSQL
- HuggingFace embeddings

