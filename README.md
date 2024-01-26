# Knowledge Graph from Text Project

This project demonstrates how to create a knowledge graph from textual data using various Python libraries. The script processes text data, identifies named entities, resolves coreferences, and constructs a graph representing relationships between entities.

## Installation

Before running the script, you need to install the necessary Python libraries. You can do this via pip. Here are the libraries used in the project:

- `wikipedia` for accessing and parsing data from Wikipedia.
- `spacy` and `spacy-transformers` for natural language processing tasks like named entity recognition and coreference resolution.
- `networkx` for creating and manipulating complex graphs.
- `pyvis` for visualizing the graph.

You can install these libraries using the following commands:

```bash
pip install wikipedia
pip install spacy spacy-transformers
pip install networkx
pip install pyvis
python -m pip install coreferee
python -m coreferee install en
```

Additionally, you need to download the language model for spaCy. Run the following command:

```bash
python -m spacy download en_core_web_lg
```

## Running the Script

To run the script, simply execute it with Python. Ensure that you have all the dependencies installed as mentioned above.

```bash
python src/knowledge_graph.py
```

The script will output data at various stages of processing and will generate a graph, which will be displayed as an HTML file (`example.html`).

## Notes

- The script is configured to extract and process text related to 'New York'. You can modify the `title` variable in the script to process a different Wikipedia page.
- The graph visualization is interactive and can be viewed in a web browser.
