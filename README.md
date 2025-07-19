# RAG (Retrieval Augmented Generation) Healthcare Guide

A Jupyter notebook-based RAG system that uses Google's Gemini AI to answer questions about healthcare documents. The system loads PDF documents, creates embeddings, and provides intelligent question-answering capabilities.

## Features

- PDF document loading and processing
- Text chunking with overlap for better context retention
- Vector embeddings using Google's Gemini embedding model
- FAISS vector store for efficient similarity search
- Question-answering using Gemini 2.5 Pro model
- Interactive chat interface

## Prerequisites

- Python 3.8 or higher
- Google API key for Gemini AI
- Jupyter Notebook or JupyterLab

## Installation

1. Clone this repository:

```bash
git clone https://github.com/samyakraka/RAG-Langchain/
cd RAG
```

2. Install required packages:

```bash
pip install -r requirements.txt
```

3. Create a `.env` file in the project root and add your Google API key:

```
GOOGLE_API_KEY=your_api_key_here
```

## Usage

1. Open the Jupyter notebook:

```bash
jupyter notebook RAG.ipynb
```

2. Place your PDF file in the project directory and update the file path in the notebook

3. Run all cells to initialize the RAG system

4. Use the interactive chat interface to ask questions about your healthcare document

## Configuration

- **Chunk size**: 1000 characters with 200 character overlap
- **Embedding model**: models/embedding-001
- **LLM model**: gemini-2.5-pro
- **Vector store**: FAISS

## Security

- Never commit your API keys to version control
- Use environment variables for sensitive information
- The `.env` file is included in `.gitignore`

## File Structure

```
RAG/
├── RAG.ipynb           # Main Jupyter notebook
├── requirements.txt    # Python dependencies
├── README.md          # This file
├── .env               # Environment variables (not tracked)
├── .gitignore         # Git ignore file
└── content/
    └── Healthcare_guide_proper.pdf  # Sample healthcare document
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License.
