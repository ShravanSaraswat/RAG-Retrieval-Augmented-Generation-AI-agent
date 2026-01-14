# RAG PDF Chat App

This repository contains a production-ready **Retrieval-Augmented Generation (RAG)** application built in Python that lets users upload PDFs and ask natural language questions over their content through a Streamlit web UI.[web:22] The backend combines FastAPI, Qdrant, LlamaIndex, Inngest, and OpenAI to deliver reliable, observable AI workflows suitable for real-world deployment.[web:22][web:23]

## Features

- Upload one or more PDF documents and query them via a chat-style interface.[web:22]  
- LlamaIndex-based PDF loading, chunking, and indexing into a Qdrant vector database for fast similarity search.[web:22][web:23]  
- OpenAI models for answer generation grounded in retrieved document context to reduce hallucinations.[web:22]  
- Inngest orchestration with retries, logging, and detailed run history for AI workflows.[web:22]  
- FastAPI backend endpoints, easily extendable or integrable with other services and UIs.[web:22]  

## Tech Stack

- **Backend:** FastAPI, Inngest, OpenAI SDK[web:22]  
- **Vector DB:** Qdrant (running locally via Docker)[web:23]  
- **Indexing:** LlamaIndex for PDF ingestion and chunking[web:23]  
- **Frontend:** Streamlit web app[web:22]  

## Getting Started

1. Clone the repository and install dependencies with your preferred Python environment manager.  
2. Run Qdrant locally (Docker) and ensure it is available on `localhost:6333`.[web:23]  
3. Create a `.env` file with your `OPENAI_API_KEY`.  
4. Start the FastAPI backend with Uvicorn.  
5. Launch the Streamlit app and open it in your browser to upload PDFs and start chatting.[web:22]  

You can adapt this template by swapping models, changing chunking parameters, or pointing to a managed Qdrant instance for production use cases.[web:23]
