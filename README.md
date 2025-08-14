# RAG Ingestion Pipeline

## Overview
This project demonstrates the **ingestion** process for a Retrieval-Augmented Generation (RAG) system.  
Ingestion is the first stage of a RAG workflow, where raw documents are transformed into a searchable, semantically rich vector database that can power accurate, context-aware responses from a large language model (LLM).

## Features
- **Document Collection**: Load text data from APIs, file systems, or other sources (demo uses Box API).
- **Chunking**: Split text into semantically meaningful overlapping segments.
- **Metadata Enrichment**: Store document attributes like author, date, and file path.
- **Embedding Generation**: Convert chunks to dense vector representations using an embedding model.
- **Vector Indexing**: Insert vectors into a vector database for fast approximate nearest neighbor (ANN) search.

## Why Ingestion Quality Matters
- **Large Chunks** → Lost context
- **Poor Embeddings** → Irrelevant results
- **Missing Metadata** → Inability to filter or sort effectively  

## Prerequisites
- Python 3.9+

## Setup
1. Clone this repository or download the notebook file.
2. Create virtual environment.
```bash
   python3 -m venv rag_env
```
3. Activate Environment
```bash
# macOS / Linux:
source rag_env/bin/activate
# Windows (PowerShell):
rag_env\Scripts\Activate.ps1
```
4. Install dependencies:
```bash
pip install -r requirements.txt
```
