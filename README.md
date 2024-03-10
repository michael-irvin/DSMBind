# DSMBind

This is the official Github repo for the following papers:
* Jin et al., DSMBind: SE(3) denoising score matching for unsupervised binding energy prediction and nanobody design, Biorxiv 2023
* Jin et al., Unsupervised protein-ligand binding energy prediction with Neural Euler's Rotation Equations, NeurIPS 2023

# Data

The training and test data can be downloaded from https://zenodo.org/records/10402853. Please put the download data in `data/` under the root folder.

# Installation

Please make sure you install the following packages
* pytorch (tested on v1.13)
* biotite (https://www.biotite-python.org/install.html)
* SRU++ (https://github.com/asappresearch/sru)
* ESM-2 (https://github.com/facebookresearch/esm)

Once you finished these installation, please run `pip install -e .`. To install SRU++, run 
```
git clone https://github.com/asappresearch/sru
cd sru
git checkout 3.0.0-dev
pip install .
```

Also install
* chemprop (https://chemprop.readthedocs.io/en/latest/installation.html#option-2-installing-from-source)

# Inference
This notebook `tutorials.ipynb` contains all the relevation information on predicting binding energy for protein-ligand, protein-protein, and antibody-antigen complexes.
