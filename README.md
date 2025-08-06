### AI-Powered RAG System with Flask and FAISS

This project demonstrates a robust and scalable Retrieval-Augmented Generation (RAG) system built with Python, Flask, and a suite of powerful deep learning libraries. It serves as a practical, end-to-end example of how to build a conversational AI agent that can answer questions based on a custom knowledge base.

#### **Core Features:**

* **RAG Architecture:** The system leverages a RAG pipeline to combine the strengths of a powerful retrieval model (Sentence-Transformers) with a state-of-the-art generative model (Phi-3.5-mini-instruct). This architecture ensures that the AI's responses are not only coherent but also grounded in specific, verifiable information from the provided documents.
* **Efficient Vector Search with FAISS:** Documents are chunked, embedded, and indexed using FAISS, a high-performance library for similarity search. This allows for lightning-fast retrieval of the most relevant information from a large dataset, making the system highly scalable.
* **GPU Acceleration:** The entire pipeline is optimized for GPU utilization, from generating embeddings in batches to running the generative large language model (LLM). This significantly reduces processing time and enables the handling of large-scale datasets and complex queries.
* **Containerized Microservice:** The application is encapsulated in a Flask API, making it easy to deploy as a containerized microservice. This architecture allows the RAG system to be seamlessly integrated into other applications and services.
* **Reproducible Workflow:** The project includes a complete workflow for downloading, processing, and indexing data. It intelligently checks for existing data and index files, allowing for a fast and reproducible setup.
* **PubMedQA Integration:** A separate notebook is included to demonstrate the system's core functionalities by integrating and evaluating it against the labeled PubMedQA dataset. This provides a clear example of how to adapt the system for domain-specific question-answering tasks.
