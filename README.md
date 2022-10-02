# Creating a Knowledge Graph out of plain text data for semantic reasoning

### What is a knowledge graph?
In knowledge representation and reasoning, knowledge graph is a knowledge base that uses a graph-structured data model or topology to integrate data. Knowledge graphs are often used to store interlinked descriptions of entities – objects, events, situations or abstract concepts – while also encoding the semantics underlying the used terminology.

Since the development of the Semantic Web, knowledge graphs are often associated with linked open data projects, focusing on the connections between concepts and entities. They are also prominently associated with and used by search engines such as Google, Bing, and Yahoo; knowledge-engines and question-answering services such as WolframAlpha, Apple's Siri, and Amazon Alexa; and social networks such as LinkedIn and Facebook.

### Knowledge graphs out of text data

In this demo project we create a knowledge graph out of plain text data from wikipedia, extracted using the wikipedia api. After extracting the data for a specific topic, a Named Entity Recognition pretrained transformer model extracts the entities from text, which get interconnected afterwards using the Coreference Resolution technique.

### Install dependencies
_You can follow the installation steps below to run the app._

1. Clone the repo
   ```sh
   git clone https://github.com/Gent-Zambaku/nlp-knowledge-graph.git
   ```
2. Get inside the repository
   ```sh
   cd nlp-knowledge-graph
   ```
3. Create a virtual environment

   Using anaconda:
   ```sh
   conda create -n kg python==3.9.1
   conda activate kg
   ```
   Using python:
   ```sh
   pip3 install virtualenv
   python3 -m venv env
   source env/bin/activate
   ```
4. Install dependencies
   ```sh
   pip install -r requirements.txt
   ```
   or
   ```sh
   pip3 install -r requirements.txt
   

### Install NeuralCoref from source

You can install NeuralCoref from sources. (You need to already have Cython and SpaCy installed).

Here is the process:

```bash
git clone https://github.com/huggingface/neuralcoref.git
cd neuralcoref
pip install -e .
```

### Run the juppyter notebook and follow the instructions
   ```sh
   jupyter notebook
   ```
