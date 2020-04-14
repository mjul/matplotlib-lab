# Matplotlib Lab
Notebook for using Matplotlib in Python.

## Contents

- [Secondary axis with dates](secondary_axis_dates.ipynb)

# Installation

## Conda 
I am using Conda to manage Python versions and libraries and Jupyter notebooks for some of the code.

They are available from:
* [Anaconda Scientific Python](https://anaconda.org/)
* [Jupyter notebooks](https://jupyter.org/). 

The configuration of the specific environment is in the [`environment.yml`](environment.yml) file. 

### How to build the environment from `environment.yml`

You can reconstruct the environment with a single command:

    conda env create -f environment.yml

If you experience problems with the config file make sure the `enviroment.yml` file is saved with UTF-8 encoding (this 
is/was a known bug in `conda` on Windows).


### How the Environment was Initially Created 
I set up the Conda environment like so, creating a Python environment for the project with `matplotlib` and `jupyter`
notebooks:
 
    conda create --name matplotlib-lab matplotlib jupyter

The environment is activated with the `conda activate matplotlib-lab` command. 

After installing other packages with `conda install matploblib` _etc._, the `environment.yml` file 
containing the environment definition can be generated with this command:

    conda env export > environment.yml


