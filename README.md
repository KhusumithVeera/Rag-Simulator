# Rag-Simulator

Understanding RAG:

RAG (Retrieval-Augmented Generation) is a technique where relevant information is retrieved from an external knowledge source and provided to an LLM as context before the LLM generates a response.
During the ingestion phase, documents are split into chunks, and each chunk is converted into an embedding using an embedding model. These embeddings, along with the original chunk text and metadata, are stored in a vector database.
When a user asks a question, the query is converted into an embedding. The system performs a similarity search against the stored embeddings to identify the most relevant chunks.
Those retrieved chunks are then combined with the user's query and system instructions and passed to the LLM. The LLM uses the retrieved context to generate a grounded response.
