# RAG-based Llama Index Query System

This repository implements a Retrieval-Augmented Generation (RAG) system using the `llama_index` library. It allows users to query academic and research documents efficiently by integrating vector-based search with large language models (LLMs). The project is designed to provide precise and contextually relevant question-answering from academic or research-based content.

## Key Features

- **Document Ingestion**: Load academic documents (e.g., PDFs) for indexing.
- **Text Splitting**: Segment documents into manageable chunks using sentence splitting.
- **Vector-Based Retrieval**: Store document embeddings and retrieve relevant content based on similarity.
- **Customizable Query Engine**: Configure prompt templates and retrieval settings for tailored answers.
- **Prebuilt Prompts**: Use a knowledge assistant prompt template optimized for accuracy and brevity.
- **Persistent Storage**: Save and reload indexed data for efficient reuse.

## Installation

### Prerequisites

1. Python >= 3.8
2. Virtual Environment (Recommended)
3. Required Libraries:
    - `llama_index`
    - `huggingface`
    - `torch`
    - `ollama`
    - Other dependencies (see the notebooks)

### Setup

1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd <repository-directory>
    ```

2. Create and activate a virtual environment:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required libraries.

    1. **rag_llama_index_1.ipynb**
    ```sh
    pip install llama-index llama-index-embeddings-huggingface llama-index-llms-gemini
    pip install -q llama-index google-generativeai
    ```

    2. **rag_llama_index_2.ipynb**
    ```sh
    pip install llama-index llama-index-embeddings-huggingface llama-index-llms-gemini spacy
    ```

    3. **rag_llama_index_3.ipynb**
    ```sh
    pip install llama-index llama-index-embeddings-huggingface llama-index-llms-ollama
    ```

    4. **rag_llama_index_4.ipynb**
    ```sh
    pip install llama-index llama-index-embeddings-huggingface llama-index-llms-ollama
    ```


## Usage

### Running the Notebooks

1. **rag_llama_index_1.ipynb**: This notebook demonstrates setting up the embedding model and LLM, loading documents, splitting text, creating a vector store index, and querying the index.
2. **rag_llama_index_2.ipynb**: This notebook focuses on evaluating the model's performance using different chunk sizes and evaluating faithfulness and relevancy.
3. **rag_llama_index_3.ipynb**: This notebook shows how to generate question-context pairs, evaluate different embedding models, and display the results.
4. **rag_llama_index_4.ipynb**: This notebook provides a complete example of configuring the LLM and embeddings, loading documents, creating a vector store index, and retrieving answers to queries.

### Example

To run the notebooks, start Jupyter Notebook:
```sh
jupyter notebook