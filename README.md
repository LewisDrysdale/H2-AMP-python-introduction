# H2-AMP-python-introduction

Lots borrowed from [Introduction to Python](https://rabernat.github.io/research_computing/intro-to-python.html) and Max Holloway and Paola Arce's previous notes.

## Setup

### Installation instructions

#### Miniconda

Miniconda is a free minimal installer for conda.

Download Minconda [here](https://docs.conda.io/en/latest/miniconda.html)

Double click on the .exe. file and follow the instllation instructions selecting installation for **user only**

### Creating a virtual environment

Python virtual environments are used to create and manage separate environments 
for your Python projects (isolated environments for different projects). 
Python has a unique way of downloading, storing, and resolving packages (or modules).

We'll create a python environment with the neccessary dependencies to do some work. 

We can setup the environemnt in one of two ways:

##### At the command line

Minvconda comes with Anaconda Prompt. You can find this by typing `Anaconda Prompt` into the windows search bar

Open the Anaconda prompt window and run the following code.

	conda create -n h2amp python=3.9 scipy jupyter jupyterlab numpy matplotlib pandas xarray scikit-learn

The second line of code activates the new environment.

	conda activate h2amp

##### Using a .yml file

You can list the modules you require and their dependencies in a text file called `environment.yml`.I have masde one for you.
It also contains the name of your environment. 
This file can be used to create your virtual environment by entering the folowing code.

	conda env create -f environment.yml
	
You can verfiy your environment has been created by typing

	conda env list
	
Now activate your new environment

	conda activate h2amp
	
### Start programming	

#### Opening Jupyter

[Jupyter](https://jupyter.org/) is a web-based interactive computing platform that we can use to write, read, run, and edit Python scripts. 
There are many others available such as [Spyder](https://www.spyder-ide.org/), [PyCharm](https://www.jetbrains.com/pycharm/) 

To open Jupyter, we can just write the following in the Anaconda Prompt

	jupyter lab
