# RAG-based-Q-A-System

Chat with Multiple PDFs using RAG and FAISS

A Python Streamlit app that allows you to upload multiple PDF documents and ask questions. This project demonstrates a Retrieval-Augmented Generation (RAG) approach using FAISS for vector-based document retrieval and Google Generative AI for answering questions based on context.

## Features

- Upload multiple PDF files.
- Extract text from PDFs and split into chunks.
- Create vector embeddings for chunks using Google Generative AI Embeddings.
- Store embeddings in FAISS for fast similarity search.
- Ask questions and get answers from uploaded documents.
- RAG pipeline: retrieves relevant chunks and generates context-aware answers.

## What is FAISS?

FAISS is an open-source library developed by Facebook AI for efficient similarity search and clustering of dense vectors.  
It’s widely used in applications like semantic search, recommendation systems, and RAG systems.

In our project, FAISS is used to store vector embeddings of PDF text chunks and quickly retrieve the most relevant chunks based on a user query.

## Installation

### Clone the repository

```bash
git clone https://github.com/ThangaKumarC/RAG-based-Q-A-System.git
cd RAG-based-Q-A-System
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Set your API key

Create a `.env` file in the root folder:

```
GOOGLE_API_KEY=your_google_api_key_here
```

### Run the Streamlit app

```bash
streamlit run app.py
```
