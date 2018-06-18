# SciPy 2018 JupyterLab tutorial.

This repository contain material and instructions to follow the "Getting started with JupyterLab" tutorial during SciPy 2018.

During the tutorial, feel free to get on the `jupyterlab` channel of scipy2018.slack.com for help and updates.

# Installation

Please read the following section and install the required software ahead of
time. We may ask you to update versions of the software more closely to the
tutorial date.

Please do not rely on cloud hosting to follow this tutorial, as the network
connection may be unreliable. If possible, come to the tutorial with a computer
where you have administrative privileges.

We'll assume you are using a recent Anaconda Python distribution (such as Anaconda or
Miniconda). If you choose to work with a different Python distribution, we'll do
our best to help you, but you may have to solve any difficulties on your own.

## Software installation

1. Install either the full [anaconda
   distribution](https://www.anaconda.com/download/) (very large, includes lots
   of conda packages by default) or
   [miniconda](https://conda.io/miniconda.html) (much smaller, with only
   essential packages by default, but any conda package can be installed).

2. Create a conda environment:

```
# Create the conda environment with specific packages
conda create -n scipy18jlab -c conda-forge --yes python=3.6 pip cookiecutter=1.6 notebook=5.5  pandas=0.23 nodejs=9.11 jupyterlab bqplot ipyvolume pythreejs

# Activate the conda environment
conda activate scipy18jlab

# Install extra JupyterLab extensions
jupyter labextension install @jupyter-widgets/jupyterlab-manager jupyter-threejs ipyvolume bqplot @jupyterlab/geojson-extension @jupyterlab/fasta-extension
```

If you open multiple terminal windows make sure to activate the environment in each of them.

## Tutorial materials

To get the tutorial materials, clone this repository. **Please plan to update the materials shortly before the tutorial.**

```
git clone https://github.com/jupyterlab/scipy2018-jupyterLab-tutorial
```

To update the materials:
```
$ cd scipy2018-jupyterLab-tutorial
$ git pull
```

Feel free to open an issue or send a pull request to update these materials if things are unclear.
