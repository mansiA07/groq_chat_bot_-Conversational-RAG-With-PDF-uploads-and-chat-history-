📄 Conversational RAG Q&A with PDF Upload & Chat History

This is a Conversational RAG (Retrieval-Augmented Generation) app built with Streamlit, allowing users to upload PDF documents and interact with their contents via natural language queries. It maintains chat history across sessions, reformulates context-aware questions, and provides concise, accurate answers using Groq's Gemma2-9b-It model.

🚀 Features

✅ Upload one or multiple PDFs.

✅ Ask questions about the content.

✅ Maintains per-session chat history.

✅ Context-aware question reformulation.

✅ Powered by HuggingFace embeddings + Groq LLMs.

✅ Built with LangChain + Streamlit.

🧠 Tech Stack
Component	Description
🧠 LLM	Groq API (Gemma2-9b-It)
🔍 Embeddings	HuggingFace all-MiniLM-L6-v2
🧱 Vector DB	ChromaDB (in-memory)
📄 PDF Loader	PyPDFLoader from langchain_community
💬 Chat History	ChatMessageHistory per session
🖥️ Frontend	Streamlit
```
Langchain-project/
└──RagQnA/
    ├── Chat_pdf_app.py     # Main Streamlit app
    ├── .env                # HuggingFace token stored here
    └── temp.pdf            # Temporary PDF used during processing
```
⚙️ Setup Instructions
1. Clone the Repo
bash
```
git clone https://github.com/yourname/pdf-chat-rag-app.git
cd Langchain-project/4-RagQnA
```
2. Create a Virtual Environment
bash
```

python -m venv venv
venv\Scripts\activate   # On Window
```
3. Install Dependencies
bash
```

pip install -r requirements.txt
```
🏁 Run the App
bash
```
streamlit run Chat_pdf_app.py
```
🖼️ UI Preview

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4d7454d6-eecb-4c74-9248-efe3670b69b8" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7877661a-38ac-414f-9401-f46374b9db39" />

