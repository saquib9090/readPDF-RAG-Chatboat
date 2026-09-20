# PDF RAG Chatbot

A Retrieval-Augmented Generation (RAG) chatbot that allows users to upload PDF documents and ask questions about their content.

The application retrieves relevant information from the uploaded PDF and uses a Large Language Model (LLM) to generate answers based on the retrieved context.

##  Project Overview

This project demonstrates how RAG can be used to build a document-based question-answering system.

Instead of sending the entire PDF to an LLM, the system:

1. Loads the PDF document
2. Extracts the text
3. Splits the text into smaller chunks
4. Converts the chunks into embeddings
5. Stores the embeddings in a vector database
6. Retrieves relevant chunks based on the user's question
7. Sends the retrieved context to the LLM
8. Generates a relevant answer

## Architecture

```text
PDF Document
     ↓
Document Loader
     ↓
Text Splitting
     ↓
Embeddings
     ↓
Vector Database
     ↓
Retriever
     ↓
Relevant Context
     ↓
LLM
     ↓
Answer
```

## 🛠️ Technologies Used

* Python
* LangChain
* OpenAI / LLM
* ChromaDB
* PyPDF
* Streamlit
* Vector Embeddings
* Retrieval-Augmented Generation (RAG)

## Project Structure

```text
pdf-rag-chatbot/
│
├── data/
│   └── sample.pdf
│
├── src/
│   ├── __init__.py
│   ├── document_loader.py
│   ├── text_splitter.py
│   ├── embeddings.py
│   ├── vector_store.py
│   ├── rag_pipeline.py
│   └── app.py
│
├── .env
├── .gitignore
├── requirements.txt
├── README.md
└── main.py
```

## How to Run

The application will be run using Streamlit:

```bash
streamlit run src/app.py
```

## Current Status


 **Project in progress**

Currently working on the PDF document loading and RAG pipeline.

## 🔮 Future Improvements

* Support multiple PDF documents
* Display source citations for answers
* Add conversation history
* Add document management
* Add user authentication
* Add role-based access control (RBAC)
* Deploy the application to the cloud

## Author

**Mohammad Saquib**

AI/ML & Generative AI Enthusiast
