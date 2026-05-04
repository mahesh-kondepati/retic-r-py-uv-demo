# Reticulate-r-python demo using UV

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

This is a short demo of reticulate to create a bilingual project using alternating r and python code chunks within .qmd file. Not sure if we can create a .qmd file successfullly from ccds. Lets see! We will use lemur-data from tidytuesday. This demo is a customised replica of the Nicola Rennies blog post (url: https://nrennie.rbind.io/blog/combining-r-and-python-with-reticulate-and-quarto/). Additionally, I am testing the reproducibility by using .renv (for r) and conda (for python) for package and environment management.

There was a similar repo on my git, however the difference is the use of UV as the python package manager in this repo. A quick comparison of this repo with the other (reticulate-r-py-demo) reveals that UV is super quick to impliment - not only in terms of the processing speed, but also in how simply the code could be written. A promising and reliable option for reproducibility for python-only projects which is widely known by now, and equally well for polyglot projects like this one.

## Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         Reg-Prediction and configuration for tools like black
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.cfg          <- Configuration file for flake8
│
└── Reg-Prediction   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes Reg-Prediction a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    └── plots.py                <- Code to create visualizations
```

--------

