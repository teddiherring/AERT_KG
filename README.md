**[contents](#Contents) | [setup](#Setup) | [running the notebooks](#running-the-notebooks) | [issues](#issues)**

# AERT_KG

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14037424.svg)](https://doi.org/10.5281/zenodo.14037424)

Notebook to support the publication *Continuous Monitoring of Permafrost and Active Layer Dynamics with Automated Electrical Resistivity Tomography on King George Island, Antarctica* (Herring et al., submitted to Geophysical Research Letters)

## Contents

This repository contains:

1. [notebook for data processing](./data_processing_AERT_kinggeorge.ipynb): This notebook contains code for automated filtering and inversion of the A-ERT dataset, and generates plots of climate data, ERT results, soil moisture, and temperature.
2. [data files](./data): This folder contains raw A-ERT data and site data (temperature, TDR, and climate measurements).
3. [inverted data](./inverted_data): This folder contains the inverted A-ERT data. This can be loaded quickly into the processing script to avoid re-inverting the data.
 
## Setup

Here are step-by-step instructions for running these notebooks locally on your machine:

Install Python. You can use [anaconda](https://www.anaconda.com/download/) for this.

Clone this repository by running the following in your command line:

```
git clone https://github.com/teddiherring/AERT_KG
```

Next, `cd` into the directory you just created:

```
cd AERT_KG
```

You can use the provided conda environment to set up the necessary software packages:

```
conda env create -f environment.yml
conda activate kg
```

Next, running the following command

```
jupyter notebook
```

will open a Jupyter notebook in your web browser. You can now open the data processing notebook and start running the code!

## Running the notebooks

You can run each cell in the notebook individually by pressing  `shift + enter`, or you can run the entire notebook by selecting `Cell`, `Run All` in the toolbar.

## Issues

Please [make an issue](https://github.com/teddiherring/AERT/issues) if you encounter any problems while trying to run the notebooks.
