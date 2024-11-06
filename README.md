# RAG System for PDF Processing

This project implements a **Retrieval-Augmented Generation (RAG)** system for processing scientific PDF articles. The system extracts text from PDFs, generates embeddings, retrieves relevant document chunks using FAISS, and generates answers or summaries using GPT-2.



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


## Project Structure
- `data/` - This folder holds the PDF files (e.g., `a1.pdf`, `a2.pdf`) that will be processed.
- `output/` - Stores the embeddings and any generated answers or summaries.
- `src/` - Contains Jupyter notebooks for each core step of the RAG pipeline:
  - **`rag_for_biomass.ipynb`**: Extracts text from PDF files using PyMuPDF.  Generates text embeddings using Sentence-Transformer. Implements FAISS-based retrieval of relevant document chunks. Generates answers using GPT-2 based on retrieved chunks.
- `requirements.txt` - Lists all required Python libraries. Install them using `pip`.


## Requirements

The following dependencies are required to run this project:

- **PyMuPDF**: For PDF text extraction.
- **Sentence-Transformer**: For generating embeddings.
- **FAISS**: For efficient similarity search and retrieval.
- **transformers**: For GPT-2 model used in answer generation.
- **torch**: For running deep learning models.

You can install all required libraries by running:

```bash
pip install -r requirements.txt
