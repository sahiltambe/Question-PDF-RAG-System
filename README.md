# Q&A Assistant with VectorStoreIndex and HuggingFace LLM

## Introduction
This project demonstrates the creation of a Q&A assistant using the `VectorStoreIndex` from `llama_index` and the HuggingFace Language Model (LLM). The assistant is designed to answer questions accurately based on provided instructions and context.

## Objectives
- Load and process documents for the Q&A system.
- Integrate a robust language model to handle queries.
- Design prompts to guide the assistant in generating accurate responses.
- Utilize embeddings for efficient information retrieval.
- Implement a query engine to manage and respond to user queries.

## Setup

### Prerequisites
- NVIDIA GPU
- Python environment with required dependencies

### Installation
1. Check GPU status:
    ```sh
    !nvidia-smi
    ```

2. Install required packages:
    ```sh
    pip install -r requirements.txt
    ```

3. Create a directory for data:
    ```sh
    !mkdir Data
    ```

### Data Preparation
Load the documents:
    ```sh
    documents = SimpleDirectoryReader("/content/Data").load_data()
    print(documents)
    ```    

### Model Integration
Login to HuggingFace and load the Mistral model:
    ```sh
    !huggingface-cli login  ## https://huggingface.co/settings/tokens
    ```   

### Results
The Q&A assistant effectively answers queries based on the provided documents, showcasing its potential for practical applications in various domains.

### Conclusion
This project highlights the integration of advanced language models and efficient data handling techniques to build a responsive Q&A assistant. The detailed implementation provides a valuable framework for developing intelligent and responsive RAG systems.




