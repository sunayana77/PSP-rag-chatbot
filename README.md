# Progressive Supranuclear Palsy (PSP) RAG Chatbot

This project implements a Retrieval-Augmented Generation (RAG) chatbot specialized in **Progressive Supranuclear Palsy (PSP)** using LangChain, Pinecone vector database, and Groq-hosted LLaMA 3 model.

---

## Overview

- Loads a PDF document on PSP diagnosis and management.
- Splits the document into chunks for efficient retrieval.
- Embeds chunks with HuggingFace embeddings.
- Indexes vectors in Pinecone for fast similarity search.
- Uses a Groq-hosted LLaMA 3 model for conversational AI.
- Maintains chat history using LangChain's conversation memory.
- Answers questions concisely (max 2 sentences).
- Responds with "I don't know" if answer is not found.

---

## Setup & Requirements

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   
2. Required API keys:
Pinecone API key (set in environment variable PINECONE_API_KEY)
Groq API key (used in the ChatGroq LLM initialization)

3. Create a .env file where all your api key are stored.

