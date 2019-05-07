# WCAI Workshot

This is the [WCAI workshop](https://events.wharton.upenn.edu/wcai-conference/agenda/) Jupyter notebook with code and walkthrough.

## Requirements
For ease of use install Anaconda to create an enviornment to contain all the required packages that we will use and activate it.
```bash
conda create -n wcai python=3.6
source activate wcai
```

Install packages:
```bash
conda install --file requirements.txt
```

Install igraphs. If you have OSX then you might run into an error in which case you can try brewing first:
```bash
brew install igraph
```

In conda you can install igraphs using:
```bash
conda install -c conda-forge python-igraph 
```

Install required packages.

Make sure our Conda environment is available as a kernel in Jupyter notebooks:
```bash
conda install nb_conda_kernels
python -m ipykernel install --user --name wcai --display-name "Python (wcai_36)"
```
