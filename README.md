
# Retrieval-Augmented Generation (RAG) System for Scientific Articles

## Overview

This repository implements a **Retrieval-Augmented Generation (RAG)** system designed to extract information from scientific articles in PDF format, generate embeddings, perform document retrieval, and produce answers or summaries using GPT-2.

The system focuses on extracting and processing text from PDFs, embedding the text into vectors, retrieving relevant document chunks with FAISS, and using a GPT-2 model for answer generation.


## Project Structure
- `data/` - This folder holds the PDF files (e.g., `a1.pdf`, `a2.pdf`) that will be processed.
- `output/` - Stores the embeddings and any generated answers or summaries.
- `src/` - Contains Jupyter notebooks for each core step of the RAG pipeline:
  - **`rag_for_biomass.ipynb`**: Extracts text from PDF files using PyMuPDF.  Generates text embeddings using Sentence-Transformer. Implements FAISS-based retrieval of relevant document chunks. Generates answers using GPT-2 based on retrieved chunks.
- `requirements.txt` - Lists all required Python libraries. Install them using `pip`.

## Prerequisites and Requirements

Before running the code, make sure you have the following:

- **Python**: Version 3.6 to 3.10 (compatible with faiss-gpu).
- **PyMuPDF**: For efficient PDF text extraction.
- **Sentence-Transformers**: For generating sentence embeddings using the all-MiniLM-L6-v2 model.
- **FAISS**: For efficient similarity search and retrieval.
- **Transformers**: For natural language processing tasks using GPT2LMHeadModel and GPT2Tokenizer for answer generation.


### Install dependencies

You can install the required libraries using:
pip install -r requirements.txt





