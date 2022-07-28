# graphGym-Molnet
Work as part of ANL summer 2022 research with emphasis on utilizing GraphGym + DeepHyper to perform HPO on graph neural networks.

## About
The emphasis of the project is on Graph representation learning using Transformers. Leveraging the work from [Recipe for a General, Powerful, Scalable Graph Transformer](https://arxiv.org/pdf/2205.12454.pdf), this project attempts to utilize the Positional Encoders, and Structural Encoders provided in `GraphGPS` and benchmark various molecular property prediction datasets. The contribution of this project is to provide an integration of `GraphGPS` with [DeepHyper](https://github.com/deephyper/deephyper), in order to have a GNN pipelines ready for Hyperparamter Optimization.

## Packages

- `PyTorch`
- `PyTorch-Geometric`
- `DeepHyper`

```shell
# Install Pytorch
pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu116

# Install Pytorch Geometric
pip install -q torch-scatter -f https://data.pyg.org/whl/torch-${TORCH}.html
pip install -q torch-sparse -f https://data.pyg.org/whl/torch-${TORCH}.html
pip install -q git+https://github.com/pyg-team/pytorch_geometric.git

# Install DeepHyper
conda install gxx_linux-64 gcc_linux-64
pip install pip --upgrade
pip install -q deephyper["analytics"]

# Install rdkit for the datasets
pip install -q rdkit-pypi
```

## Datasets

`MoleculetNet`: MoleculeNet is a benchmark specially designed for testing machine learning methods of molecular properties. As we aim to facilitate the development of molecular machine learning method, this work curates a number of dataset collections, creates a suite of software that implements many known featurizations and previously proposed algorithms. All methods and datasets are integrated as parts of the open source DeepChem package(MIT license).

`Reference`: https://moleculenet.org/datasets-1

`Resource`: https://pytorch-geometric.readthedocs.io/en/latest/modules/datasets.html


## Results

```
TBA
```

## Literature

- L. Rampášek, et. al, Recipe for a General, Powerful, Scalable Graph Transformer, ArXiv, arxiv:2205.12454, 2022.
- J. You, et. al, Design Space for Graph Neural Networks, ArXiv, arxiv:2011.08843, 2021.

## Author
[Akhil Pandey](https://github.com/akhilpandey95)

## Supervisor
[Prasanna Balaprakash](https://github.com/pbalapra)

