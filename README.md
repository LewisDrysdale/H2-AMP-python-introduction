# H2-AMP-python-introduction

Lots borrowed from [Introduction to Python](https://rabernat.github.io/research_computing/intro-to-python.html) and Max Holloway and Paola Arce's previous notes.

## Setup

### Installer 

#### Miniconda

From the website:

***Miniconda is a free minimal installer for conda. It is a small, bootstrap
version of Anaconda that includes only conda, Python, the packages they depend
on, and a small number of other useful packages, including pip, zlib and a
few others. Use the `conda install` command to install 720+ additional conda
packages from the Anaconda repository.***

Minconda can be downloaded [here](https://docs.conda.io/en/latest/miniconda.html)

### Set up the environment using Conda

Python virtual environments are used to create and manage separate environments 
for your Python projects (isolated environments for different projects). 
Python has a unique way of downloading, storing, and resolving packages (or modules).

We can setup the environemnt in one of two ways

First we'll create a python environment with the neccessary dependencies to do some work. 
We will run the following code in your Anaconda Prompt window (a terminal provided with the Anaconda package).

We will use conda to do this but you could also use pip or easy_install. 
I find conda and the anaconda distribution easiest and most transparent for managing your python distribution.

The second line of code activates the new environment and the third line opens a jupyter notebook.

`conda create -n h2amp python=3.6 scipy jupyter numpy matplotlib pandas xarray scikit-learn`

`conda activate h2amp jupyter notebook`
