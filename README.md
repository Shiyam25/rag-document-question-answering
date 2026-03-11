# RAG-Based Document Question Answering System

## Overview

This project implements a Retrieval Augmented Generation (RAG) pipeline that answers questions from a PDF document.

The system extracts text from a document, splits it into chunks, converts them into embeddings using Sentence Transformers, and stores them in a FAISS vector database. When a user asks a question, the system retrieves the most relevant chunks and uses a HuggingFace question-answering model to generate the answer.


## Dataset

The dataset used in this project is a PDF document related to a solar inverter project.

File included in this repository:
solar_inverter_project_document.pdf

The text from this document is extracted and processed to build the retrieval system.


## Technologies Used

* Python
* Sentence Transformers
* FAISS
* HuggingFace Transformers
* NumPy
* PyPDF


## Project Workflow

1. Load the PDF document
2. Extract text using PyPDF
3. Clean the extracted text
4. Split the text into smaller chunks
5. Generate embeddings using SentenceTransformer
6. Store embeddings in a FAISS vector database
7. Convert user query into embedding
8. Retrieve the most relevant document chunks
9. Generate answers using a DistilBERT question-answering model


## Files in this Repository

rag_document_question_answering.ipynb – Jupyter notebook containing the full RAG implementation
solar_inverter_project_document.pdf – Document used for retrieval and question answering
README.md – Project documentation


## Example Questions

* What is the purpose of the solar inverter project?
* What components are used in the project?
* What is the objective of the system?


## Conclusion

This project demonstrates how Retrieval Augmented Generation (RAG) can be used to build a document-based question answering system by combining embeddings, vector search, and transformer-based language models.
