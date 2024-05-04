# arize-rag-eval-rm-thesis
A simple example of how we can evaluate LLM RAG Applications with Arize Phoenix.

This repository walks through simple chunking to build a basic RAG application with its focus mainly being on how to effectively evaluate RAG pipelines. 

Arize Phoenix is an open-source library which allows for direct traceability/observability in a web UI. As an example, a .pdf is chunked and loaded, then questions are asked against retrieved context to the LLM.

## Instructions on how to get started with Arize Phoenix in this repository:

1. File explanation:

     ```honors_thesis.pdf```: example .pdf file used in this repository for RAG.
   
     ```phoenix_evaluator.ipynb```: main python notebook.
   
     ```requirements.txt```: dependencies needed to run this notebook, ideally installed in virtual environment.
   
     ```questions_with_document_chunk.csv```: CSV file of LLM generated questions added here for convenience, optionally this can be created in the notebook.

2. Begin by creating a virtual environment, be sure to install the dependencies listed in ```requirements.txt```:

    ```python3 -m venv <myenvname>```
    
    ```pip install -r requirements.txt```

3. Run the python notebook, ```phoenix_evaluator.ipynb``` which also walks through building the RAG pipeline, interacting with the Web UI, and exporting evaluation metrics.

   In the notebook, we can start the Web interface with: ```px.launch_app()```

   The Web UI is accessible at http://localhost:6006/


------------------------------------------------------------------------------------------------------------------------------------


Reference documentation and additional examples right from Arize Phoenix can be found [here](https://docs.arize.com/phoenix).
