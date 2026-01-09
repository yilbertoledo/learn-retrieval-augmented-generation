# learn-retrieval-augmented-generation

A practical example of Retrieval Augmented Generation (RAG) for music recommendation. This project demonstrates how to use semantic search with vector embeddings to find songs based on lyrical themes, then generate recommendations using a local Large Language Model.

## Features

- **Semantic Search**: Uses sentence transformers to create embeddings of song lyrics
- **Vector Database**: Stores embeddings in Qdrant for efficient similarity search
- **Local LLM**: Generates recommendations using Ollama (runs entirely offline)
- **End-to-End RAG**: Combines retrieval (vector search) with generation (LLM) for contextual recommendations

## Tech Stack

- **Python 3.11+** with Jupyter Notebooks
- **Qdrant**: Vector database for storing embeddings
- **Sentence Transformers**: For creating text embeddings
- **Ollama**: Local LLM for generating recommendations
- **Pandas**: Data processing


## Setup

**Linux/Mac:**
```bash
python3 -m venv .venv
source .venv/bin/activate
.venv/bin/pip install -r requirements.txt
```

**Windows (PowerShell):**
```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
.venv\Scripts\pip install -r requirements.txt
```

**Windows (Command Prompt):**
```cmd
python -m venv .venv
.venv\Scripts\activate.bat
.venv\Scripts\pip install -r requirements.txt
```

**Note:** If you encounter an execution policy error in PowerShell, run:
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```
