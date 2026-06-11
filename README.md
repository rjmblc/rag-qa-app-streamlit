# rag-qa-app-streamlit

A Retrieval-Augmented Generation (RAG) Question Answering application built using Streamlit, LangChain, ChromaDB, and LLMs. The application ingests PDF documents, generates vector embeddings, stores them in a vector database, and retrieves context-aware answers using semantic search.



# Features

* PDF document ingestion
* Semantic document retrieval
* Vector embeddings with HuggingFace
* ChromaDB vector storage
* LLM-powered question answering
* Interactive Streamlit UI
* Retrieval-Augmented Generation (RAG) pipeline



# Tech Stack

* Python
* Streamlit
* LangChain
* ChromaDB
* HuggingFace Embeddings
* PyMuPDF
* Groq / OpenAI LLMs



# Project Structure

```bash id="2a1vtx"
rag-qa-app-streamlit/
│
├── docs_dir/
├── vector_db/
├── app.py
├── rag_utility.py
├── requirements.txt
└── README.md
```



# Installation

## Clone Repository

```bash id="rk3c2l"
git clone https://github.com/rjmblc/rag-qa-app-streamlit.git
cd rag-qa-app-streamlit
```



# Create Virtual Environment

```bash id="lf8v3h"
python -m venv .venv
```

Activate environment:

### Windows

```bash id="5rz5o4"
.venv\Scripts\activate
```

### Linux / Mac

```bash id="5l9e0q"
source .venv/bin/activate
```



# Install Dependencies

```bash id="ntjlwm"
pip install -r requirements.txt
```



# Environment Variables

Create a `.env` file in the project root.

## Using Groq

```env id="jlwm113"
GROQ_API_KEY=your_groq_api_key
```

## Using OpenAI

```env id="jlwm114"
OPENAI_API_KEY=your_openai_api_key
```



# Add Documents

Place PDF documents inside:

```bash id="jlwm115"
docs_dir/
```



# Run the Application

```bash id="jlwm116"
streamlit run app.py
```



# Example Questions

```text id="jlwm117"
What is the Uric Acid result in the report?

Summarize the medical report.

What abnormalities are present in the document?
```



# RAG Workflow

```text id="jlwm118"
PDF Documents
      ↓
Document Loader
      ↓
Text Chunking
      ↓
Embeddings Generation
      ↓
ChromaDB Vector Storage
      ↓
Semantic Retrieval
      ↓
LLM Response Generation
```


# Future Improvements

* Multi-document retrieval
* Conversational memory
* Citation-based responses
* Hybrid search
* Agentic RAG workflows
* FastAPI backend deployment

# Author

Rajmohan Balachandran

GitHub:
https://github.com/rjmblc

# License

This project is intended for educational and learning purposes.

