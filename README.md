AI-Powered PDF Chatbot using RAG

 Overview
This project is an AI-powered PDF chatbot that allows users to upload multiple PDF documents and ask questions about their content. It uses Retrieval-Augmented Generation (RAG) to retrieve relevant information from uploaded documents and generate context-aware answers.

The application is built with Python, LangChain, LangGraph, Groq, Google Gemini Embeddings, and Streamlit.

 Key Features
- Multiple PDF Uploads: Upload and process multiple PDF documents.
- Document Processing: Extract text from PDFs using PyPDFDirectoryLoader.
- Text Chunking: Split large documents into smaller chunks using RecursiveCharacterTextSplitter.
- Vector Embeddings: Convert document chunks into embeddings using Google's Gemini Embedding model.
- Semantic Search: Retrieve the top 3 most relevant document chunks using InMemoryVectorStore.
- AI-Powered Responses: Generate answers using the Groq-hosted GPT-OSS-20B model.
- Conversational Memory: Maintain conversation context using LangGraph's InMemorySaver.
- Interactive Chat Interface: Chat with uploaded documents through Streamlit.

 Tech Stack
- Programming Language: Python
- Frontend: Streamlit
- AI Framework: LangChain and LangGraph
- LLM: GPT-OSS-20B via Groq
- Embedding Model: Google Gemini Embedding-001
- Vector Database: InMemoryVectorStore
- Document Loader: PyPDFDirectoryLoader
- Memory: LangGraph InMemorySaver

 How It Works
1. Users upload one or more PDF documents.
2. The application extracts text from the uploaded PDFs.
3. The extracted text is divided into smaller chunks.
4. Google Gemini Embeddings converts the chunks into vector representations.
5. The vectors are stored in an in-memory vector database.
6. When a user asks a question, the AI agent can retrieve relevant document content using a custom retrieval tool.
7. The LLM generates a response using the retrieved information.
8. Conversation history is maintained to support follow-up questions.

 What I Learned
Through this project, I gained hands-on experience with Retrieval-Augmented Generation (RAG), document processing, vector embeddings, semantic search, AI agents, conversational memory, and building interactive AI applications using Streamlit.

 Future Improvements
- Add source citations and page references.
- Support additional file formats such as DOCX and TXT.
- Integrate ChromaDB for persistent vector storage.
- Improve retrieval accuracy and response reliability.
- Add document management and chat reset functionality.
