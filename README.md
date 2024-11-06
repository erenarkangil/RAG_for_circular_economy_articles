# RAG_for_scientific_Articles
Rag tutorial how to make chatbot for bioeconomy articles


# Retrieval-Augmented Generation (RAG) System for Scientific Articles

## Overview

This repository implements a **Retrieval-Augmented Generation (RAG)** system designed to extract information from scientific articles in PDF format, generate embeddings, perform document retrieval, and produce answers or summaries using GPT-2.

The system focuses on extracting and processing text from PDFs, embedding the text into vectors, retrieving relevant document chunks with FAISS, and using a GPT-2 model for answer generation.

## Prerequisites

Before running the code, make sure you have the following:

- Python 3.6+
- PyTorch 1.8+
- FAISS
- Sentence-Transformers
- Transformers
- PyMuPDF
- NLTK

### Install dependencies

You can install the required libraries using:

pip install -r requirements.txt
