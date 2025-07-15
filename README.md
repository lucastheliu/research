# Repository

This repository contains source code for building machine learning models with and without federated learning, as well as for analyzing the effectiveness of inversion attacks against these models.

## Description

The purpose of the source code in this repository is to demonstrate that federated learning models are more secure and better prevent the leakage of sensitive training data than conventional training models.

The federated learning model in this repository is based on **Convolutional Neural Network** architecture, while the conventional model is based on **Multilayer Perceptron**.

Both models are trained using the MNIST dataset, which contains 70,000 images of numbers ranging from zero to nine.

## Prequisites

Create a virtual environment and install the required dependencies in `requirements.txt`. The following commands may vary depending on the platform.

```zsh
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

You can view the notebook using an editor with a built-in Jupyter Notebook rendering engine (such as **VSCode** with the Jupyter Notebook extension) or by opening the notebook editor web page in the terminal.

```zsh
pip install notebook
jupyter notebook
```

## Get Started

First, open `mlp.ipynb` under the `notebooks/` directory and run each code block individually. A new directory `models/` will be created relative to the file's parent path. This directory contains all the models that the code has trained. Therefore, you won't need to retrain them when you run the inversion attack in the `attack.ipynb` notebook later.

Afterwards, you can check all the other notebooks or the `src/` directory, which contains model architectures in `models.py` and utility functions, such as those for downloading and loading the MNIST dataset, in `utils.py`.

For more information about each notebook, check the top of the notebook, where you will find details about the requirements needed to run it.

## File Structure

```
.
├── .gitignore
├── LICENSE
├── README.md
├── models
│   ├── federated_model.pth
│   └── mlp_model.pth
├── notebooks
│   ├── attack.ipynb
│   ├── federated.ipynb
│   ├── mlp.ipynb
│   └── resources
│       ├── Federated_learning_code(2).ipynb
│       ├── Federated_learning_codes(3).ipynb
│       ├── Federated_learning_codes(4).ipynb
│       ├── Federated_learning_codes(5).ipynb
│       └── Federated_learning_codes_(1).ipynb
├── requirements.txt
└── src
    ├── models.py
    └── utils.py
```

## Licensing

This repository is licensed under the **LICENSE**.
