# RAG PDF Chat App

This repository contains a production-ready **Retrieval-Augmented Generation (RAG)** application built in Python that lets users upload PDFs and ask natural language questions over their content through a Streamlit web UI.The backend combines FastAPI, Qdrant, LlamaIndex, Inngest, and OpenAI to deliver reliable, observable AI workflows suitable for real-world deployment.

## Features

- Upload one or more PDF documents and query them via a chat-style interface.
- LlamaIndex-based PDF loading, chunking, and indexing into a Qdrant vector database for fast similarity search.
- OpenAI models for answer generation grounded in retrieved document context to reduce hallucinations.
- Inngest orchestration with retries, logging, and detailed run history for AI workflows.
- FastAPI backend endpoints, easily extendable or integrable with other services and UIs.

## Tech Stack

- **Backend:** FastAPI, Inngest, OpenAI SDK
- **Vector DB:** Qdrant (running locally via Docker)
- **Indexing:** LlamaIndex for PDF ingestion and chunking
- **Frontend:** Streamlit web app

## Getting Started

1. Clone the repository and install dependencies with your preferred Python environment manager.  
2. Run Qdrant locally (Docker) and ensure it is available on `localhost:6333`.
3. Create a `.env` file with your `OPENAI_API_KEY`.  
4. Start the FastAPI backend with Uvicorn.  
5. Launch the Streamlit app and open it in your browser to upload PDFs and start chatting. 

You can adapt this template by swapping models, changing chunking parameters, or pointing to a managed Qdrant instance for production use cases.

