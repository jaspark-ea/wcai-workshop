# WCAI Workshot

This is the [WCAI workshop](https://events.wharton.upenn.edu/wcai-conference/agenda/) Jupyter notebook with code and walkthrough.

## Requirements

### Setup Conda Environment
For ease of use install Anaconda to create an enviornment to contain all the required packages that we will use and activate it.
```bash
conda create -n wcai python=3.6
source activate wcai
```

Activate the environment. If you are on OSX or Linux use 
```bash
source activate wcai
```
If you are on Windows use:
```bash
activate wcai
```

### Install Packages
Install packages:
```bash
conda install --file requirements.txt
```


### Install igraphs
The python package igraphs is a bit more involved process.

#### OSX
If you OSX then you might run into an error in which case you can try brewing first:
```bash
brew install igraph
```

In conda you can install igraphs using:
```bash
conda install -c conda-forge python-igraph 
```

#### Windows
 1. For windows, go to this link: [python-igraphs](https://www.lfd.uci.edu/~gohlke/pythonlibs/#python-igraph)
 2. Download `python_igraph‑0.7.1.post6‑cp36‑cp36m‑win_amd64.whl`
 3. Locate the download and install using pip ```pip install C:\Users\jaspark\Downloads\python_igraph-0.7.1.post6-cp36-cp36m-win_amd64.whl```


### Setup Kernel for Jupyter
Make sure our Conda environment is available as a kernel in Jupyter notebooks:
```bash
conda install nb_conda_kernels
python -m ipykernel install --user --name wcai --display-name "Python (wcai_36)"
```


### Start Jupyter
Let's start Jupyter and open the notebook in `notebooks/WCAI Workshop.ipynb`. 
Make sure that we are using the kernal for our Conda environemnt `Python (wcai_36)`