# RAG based Chatbot with Cohere's Contextual Compressor Reranking, FAISS and OpenAI

# Executive Summary
This project aims to build an advanced retrieval system using cutting-edge NLP and deep learning technologies. The system leverages LangChain, a comprehensive NLP library, and OpenAI's GPT-3.5 Turbo model for response generation. The retrieval process involves document embedding, compression, and reranking through Cohere API, ultimately delivering precise and contextually relevant answers to user queries.

## Project Overview
### 1. Objectives
The primary objectives include:
1. Implementing document loading from PDFs using LangChain's PyPDFDirectoryLoader.
2. Splitting documents efficiently into smaller chunks.
3. Utilizing Hugging Face's BAAI/bge-large-en-v1.5 for document embeddings.
4. Building a Faiss-based vector store for efficient document retrieval.
5. Enhancing retrieval results with Cohere's contextual compression reranking.
6. Integrating OpenAI's GPT-3.5 Turbo model for response generation.
7. Creating a RetrievalQA pipeline for seamless interaction with end-users.

### 2. Technologies Used
- LangChain: A comprehensive NLP library for document loading, text splitting, embeddings, and retrieval.
- OpenAI GPT-3.5 Turbo: A powerful language model for generating human-like responses.
- Cohere API: Utilized for contextual compression and reranking.
- Hugging Face Transformers: Employed for document embeddings.
- Faiss: A GPU-accelerated library for similarity searches in large datasets.

### 3. Workflow
#### Document Loading and Splitting
- PDF documents are loaded using PyPDFDirectoryLoader.
- Documents are split into smaller chunks using RecursiveCharacterTextSplitter.

#### Embedding Model
- Hugging Face's BAAI/bge-large-en-v1.5 is employed for document embeddings.
- Embeddings are computed with GPU acceleration for efficiency.

#### Vector Store (Faiss) Retrieval
- Faiss is used to build an efficient vector store for document retrieval.
- Retrieval is performed based on cosine similarity.

#### Reranking with Cohere
- Cohere API is utilized for contextual compression and reranking.
- The compression retriever enhances the quality of retrieved documents.

#### OpenAI Model Integration
- OpenAI's GPT-3.5 Turbo is used for response generation.
- The model is initialized with the provided API key.

#### RAG Pipeline with Compressor Retriever
- A RetrievalQA pipeline is created using LangChain, integrating OpenAI, Cohere, and Faiss.

#### User Interaction
- Users can interact with the system by providing queries.
- The system responds with contextually relevant answers.

### Results and Insights
The system demonstrates advanced retrieval capabilities, combining document embeddings, Faiss-based retrieval, and Cohere's contextual compression reranking. OpenAI's GPT-3.5 Turbo enhances user interactions by generating informative and coherent responses.

### Challenges and Future Work
1. Scalability: Evaluate the system's efficiency with a large dataset.
2. Model Fine-tuning: Enhance performance through fine-tuning of embedding and language models.
3. User Interface: Develop a user-friendly interface for easy interaction and integration.

### Conclusion
This project successfully integrates cutting-edge NLP and deep learning technologies, offering a powerful solution for information retrieval and user interactions. Further improvements and optimizations can be explored in future iterations of the system.
