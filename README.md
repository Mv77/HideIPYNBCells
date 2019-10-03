# HideIPYNBCells

This repository is meant as an example of how to generate new Jupyter notebooks from an original "master" Jupyter notebook, filtering which cells from the master notebook to reproduce.

The main file is [Example.ipynb](https://github.com/Mv77/HideIPYNBCells/blob/master/Example.ipynb). Each of its cells have [tags](https://blog.jupyter.org/jupyter-notebook-5-0-909c6c172d78), which are used to group cells that one might want to filter. The first cell uses *nbconvert* to generate a new notebook from which cells tagged "Answer" or "Conversion" are removed. The result is [ExampleQuestions.ipynb](https://github.com/Mv77/HideIPYNBCells/blob/master/ExampleQuestions.ipynb).

*Note:* nbconvert uses [Pandoc](https://pandoc.org/).

Examples of why this might be useful are:
- Problem sets: you can have a master file with questions and answers and automatically generate and update a file with the questions only.
- Notebooks that need to be presented in multiple languages: just keep them all in the master file and create auxiliary files for each language.
