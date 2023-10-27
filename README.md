# Exploring the Limits of Large Language Models for Word Definition Generation: A Comparative Analysis

This repository contains the code and data for the paper Exploring the Limits
of Large Language Models for Word Definition Generation: A Comparative Analysis.

If used, please cite: Exploring the Limits of Large Language Models for Word Definition Generation: A Comparative Analysis. Esteban Rodríguez Betancourt and Edgar E. Casasola.

```bibtex
@INPROCEEDINGS{RodriguezBetancourt2023,
  author={Rodríguez-Betancourt, Esteban and Casasola-Murillo, Edgar},
  booktitle={2023 XVLIV Latin American Computer Conference (CLEI)}, 
  title={Exploring the Limits of Large Language Models for Word Definition Generation: A Comparative Analysis}, 
  year={2023},
  volume={},
  number={}
}
```

## Install

To make easier to reproduce the results, the code is provided as Jupyter Notebooks.

- Clone the repo, using `git clone <repo>`
- Move into the repo, using `cd <repo>`
- If required, install virtualenv, using `pip install virtualenv`
- Create a virtual environment, using `virtualenv venv`
- Activate the virtual environment, using `source venv/bin/activate`
- Install the requirements, using `pip install -r requirements.txt`

## Configuration

It is required to provide your own API keys for Open AI and Hugging Faces. To do that just
copy the file keys_example.json into keys.json and fill the values.

## Notebooks

The notebooks are organized as follows:

- 00_definition_modeling.ipynb: Contains the prompts and code to fetch the definitions from the models.
- 01_embedding_evaluation_minilm.ipynb: Contains the code to compare the generated definitions with the reference definitions, using cosine similarity and a BERT model. Also includes the results of the manual evaluation.

## Dataset
The word dataset and examples used to generate the definitions is available in the file words.json.

## Generated definitions
The generated deinifitions are available in the files definitions-{model}.json.
