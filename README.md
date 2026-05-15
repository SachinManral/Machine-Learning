# Machine Learning

A small Python workspace for machine learning and document-processing experiments.
The project includes notebooks for loading documents, sample text/PDF data, and
dependencies for LangChain, ChromaDB, FAISS, and sentence transformers.

## Project Structure

```text
.
+-- data/
|   +-- pdf/          # Sample PDF files
|   +-- text_files/   # Sample text documents
+-- notebook/         # Jupyter notebooks and local ChromaDB data
+-- src/              # Python package source
+-- main.py           # Basic Python entry point
+-- pyproject.toml    # Project metadata and dependencies
+-- requirements.txt  # Dependency list
```

## Setup

Create and activate a virtual environment:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

Install dependencies:

```powershell
pip install -r requirements.txt
```

Or, if you use `uv`:

```powershell
uv sync
```

## Usage

Run the basic entry point:

```powershell
python main.py
```

Open the notebooks in Jupyter or VS Code:

```powershell
jupyter notebook
```

The main notebook currently in use is:

```text
notebook/pdf_loader.ipynb
```

## Notes

- Keep API keys and local secrets in `.env`.
- Generated vector database files are stored under `notebook/chroma_db/`.
- Sample documents live under `data/`.
