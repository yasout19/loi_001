# Legal Document Processing and Query System

## Overview
This notebook demonstrates a complete pipeline for parsing, processing, and querying a legal document (`loi.pdf`). It uses advanced NLP techniques and tools for semantic search and question-answering over the document content. The system leverages vector-based storage and a Large Language Model (LLM) for accurate and context-aware responses.

## Features
- **PDF Document Parsing**: Reads and processes legal documents in PDF format.
- **Text Splitting**: Breaks content into manageable chunks for embedding and storage.
- **Embeddings and Vector Storage**: Generates semantic embeddings using Hugging Face models and stores them in FAISS for efficient retrieval.
- **Query Handling**: Retrieves relevant document sections based on user queries.
- **LLM Integration**: Uses Google Generative AI (Gemini Pro) to answer questions based on retrieved context.

## Requirements
To run this notebook, install the following dependencies:
```bash
pip install langchain langchain-community langchain-core sentence-transformers pypdf faiss-cpu chromadb
pip install google-generativeai
```
## Setup
### 1/Environment Variables
Set your Google API key as an environment variable in the notebook:

```bash
import os
os.environ['GOOGLE_API_KEY'] = 'your-google-api-key'
```
### 2/ PDF File
Place the loi.pdf file in the same directory as the notebook.

