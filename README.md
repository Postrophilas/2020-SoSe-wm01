# 2020-SoSe-wm01

## Introduction

These are Jupyter notebooks for WM-01, Summer Semester 2019-2020, Faculty of
Biology, University of Freiburg.

## View at https://nbviewer.jupyter.org/github/strawlab/2020-SoSe-wm01/tree/master/

## Run interactively at https://mybinder.org/v2/gh/strawlab/2020-SoSe-wm01/master

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/strawlab/2020-SoSe-wm01/master)

## Run locally with anaconda

```
conda env create -f environment.yml
source activate wm01
jupyter notebook
```

## This course on Ilias

(TODO: add link)

## Some useful Python data science cheat sheets

- https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf
- http://www.utc.fr/~jlaforet/Suppl/python-cheatsheets.pdf

## In case matplotlib in Windows shows DLL errors:

When importing matplotlib, if you are getting an error like
`ImportError: DLL load failed: Das angegebene Modul wurde nicht gefunden` or
`ImportError: DLL load failed: The specified module could not be found`, do:

1) Open a Terminal in your `wm21` Anaconda virtual environment.
2) Inside the terminal, type this line-by-line:

```
pip uninstall pillow
pip uninstall matplotlib
conda uninstall matplotlib
conda install matplotlib
```

See [this](https://github.com/matplotlib/matplotlib/issues/14691#issuecomment-508552825)
for related information.

## Note for macOS users

Before starting `jupyter notebook` from the command line, you may like to type:

    ulimit -n 4096

This will solve [OSError: [Errno 24] Too many open files](https://github.com/jupyterlab/jupyterlab/issues/6727).
