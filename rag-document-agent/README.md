# RAG Pipeline & Chatbot (n8n)

This project implements a Retrieval-Augmented Generation (RAG) chatbot using n8n.

## Architecture
- Google Drive as document source
- Recursive text splitting and document loading
- OpenAI embeddings
- Pinecone vector database
- OpenRouter LLM for chat responses
- n8n AI Agent for orchestration

## Workflow Overview
1. Documents uploaded to Google Drive are automatically ingested
2. Files are split into chunks and embedded
3. Embeddings are stored in Pinecone
4. User queries retrieve relevant chunks
5. An LLM generates grounded responses using retrieved context

## Requirements
- n8n (self-hosted or cloud)
- OpenAI API key (for embeddings)
- OpenRouter API key (for LLM)
- Pinecone account and index

## Configuration
All credentials must be configured using n8n Credentials.
This repository does not include any API keys.

## Limitations
- Uses paid APIs (OpenAI, OpenRouter, Pinecone)
- Requires external services to be configured

## License
MIT
