# CSS Workshop: Word Embeddings for the Social Sciences

Author: Connor Gilroy

This repository contains the materials for a 1-hour work embeddings workshop to be held on 3/19/21, organized by the Computational Social Science reading group at TechnoSoc. Follow the instructions below to run the notebook, word-embeddings-workshop.ipynb. 

View a static web version of the workshop tutorial at https://ccgilroy.github.io/word-embeddings-workshop/. Introductory slides are [here](https://docs.google.com/presentation/d/1V4SaADerFMph9wB7pES76vYUWhIzvQ_LMpSyAIB6f_o/edit?usp=sharing).

## Setup

If you use [conda](https://docs.conda.io/en/latest/) to manage your Python environments, you can install the key packages you need for this work shop by running this command in your terminal:

```
conda env create -f environment.yml
```

The whatlies package isn't available through conda. For the optional part of the workshop that uses whatlies, install it with `pip install whatlies` (after activating the conda environment!). 

To open the notebook from your terminal, first activate the new environment, then run `jupyter lab`: 

```
conda activate emb-workshop
jupyter lab
```

---

(Here's the full code to create the conda environment. If creating it from the environment file works, you won't need this.)

```
conda create -n emb-workshop
conda activate emb-workshop
conda config --env --add channels conda-forge
conda config --env --set channel_priority strict
conda install python=3.8 jupyterlab gensim scikit-learn 
# optional, to use whatlies
pip install whatlies
```
