# Agentic-ai

A hands-on workspace for exploring agentic AI concepts, Pydantic data validation, and LangChain/LangGraph LLM orchestration.


## Project Structure

- `1-python-pydantic/`
  - `pydantic.ipynb`: Pydantic basics, data validation, and model usage in Python.
  - `python.ipynb`: Additional Python and Pydantic examples.
- `2-lang-chain-basics/`
  - `.env`: API keys for OpenAI, Groq, LangChain, etc.
  - `gettingstartedlangchain.ipynb`: LangChain introduction, prompt engineering, output parsers, LLM integration.
  - `2.1-DataIngestion/`
    - `dataingestion.ipynb`: Data/document loading and ingestion workflows.
    - `records.xml`, `speech.txt`, `syllabus.pdf`: Example data files.
  - `2.2-DataTransformer/`
    - `2.2.1-Recursivetextsplitter.ipynb`: Text splitting and transformation.
    - `records.xml`, `speech.txt`, `syllabus.pdf`: Example data files.
  - `2.3-Embeddings/`
    - `2.3.1-embeddings.ipynb`: Embedding generation with OpenAI.
    - `2.3.2-hugginface.ipynb`: Embedding generation with HuggingFace.
    - `speech.txt`: Example data file.
  - `2.4-VectorDatabase/`
    - `FAISS/`
      - `code.ipynb`: Vector database (FAISS) usage and retrieval-augmented generation.
- `3-langgraph/`
  - `langgraph_intro.ipynb`: Introduction to LangGraph for agentic workflows.
  - `tools.ipynb`: Tool and utility demonstrations.

## Requirements

Install dependencies with:

```sh
pip install -r requirements.txt
```

## Environment Setup Commands (Agentic-AI)

**Python 3.12.7:**

### Using venv (standard Python)
```sh
python -m venv myenv
```

### Using conda (in Anaconda3 folder)
```sh
conda create -n venv_ur_name python=3.12 -y
conda activate venv_ur_name
conda deactivate
conda remove -n venv_ur_name --all
```

### Using conda (in current folder)
```sh
conda create -p ./venv_ur_name python=3.12 -y
conda activate ./venv_ur_name
conda deactivate
# To delete: remove the folder venv_ur_name
```

### Creating conda environment (named)
```sh
conda create -n agentic_2_base python=3.11
conda activate agentic_2_base
```

### Creating conda environment (custom path)
```sh
# For current directory
conda create -p ./abcd001 python=3.11

# For directory of choice
conda create -p /absolute/path/to/abcd002 python=3.11
```

### Activating conda environment created with -p
```sh
conda activate /absolute/path/to/abcd002
```

## Requirements File Management

```sh
# Create requirements.txt
pip freeze > requirements.txt

# List installed packages
pip list

# Export list in freeze format
pip list --format=freeze > req.txt

# Install from requirements file
pip install -r file_name.txt
```

## Usage

1. Set up your API keys in `2-lang-chain/.env`.
2. Open the notebooks in Jupyter or VS Code.
3. Run the cells to explore Pydantic models and LangChain LLM workflows.

## Notebooks Overview

- **Pydantic Notebooks:**  
  Python data validation, type enforcement, and model nesting using Pydantic.

- **LangChain Notebooks:**  
  Prompt templates, output parsers (JSON, XML, YAML), LLM integration (OpenAI, Groq), data ingestion, transformation, embeddings, and vector database (FAISS).

- **LangGraph Notebooks:**  
  Agentic workflow orchestration and tool usage.

## License

This project is for educational purposes.