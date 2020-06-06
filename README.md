# police-shooting-data-workspace + Docker
Just a workspace where I will work on some data crunching with dockerized Jupyter notebooks.

## HOWTO In 5-minutes

Start it by running this command from root of project folder `docker-compose up`  or  `docker-compose up -d`

Once started, the former command (see Docker console output via "Docker Dashboard") will tell you the approximate URL you 
need to login to the Jupyter notebook instance.

Something like this:  

    http://localhost:8888/?token=<<unique-id>>

Once inside, open the Notebook called `Julia_Police-Shootings-Demo.ipynb` and run it one step at a time.  NOTE: The first time you
run that notebook, it might take a handful of minutes installing some stuff on the first step in the workbook where the Pkg.add 
statements are located.

At the end of 2 of the notebooks is a graphing functionn to plot data on a graph.

If you are a beginner, you might want to read this:
1. For Julia: https://docs.julialang.org/en/v1/manual/getting-started/
2. For R: https://support.rstudio.com/hc/en-us/articles/201141096-Getting-Started-with-R

## How to use this project

1.  Fork my project to your GitHub account.
2.  Add your own new separate Notebook file.  Probably you should prefer R over Julia.
3.  Create your Graphs
4.  Make a pull request and I will approve and merge it into this project.
5.  George Floyd



## Source Data

https://github.com/djangofan/police-shooting-data-workspace

## Info On Jupyter

https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html#jupyter-datascience-notebook


### What is included here in the Jupyter stack?

Using: docker pull jupyter/datascience-notebook


    Minimally-functional Jupyter Notebook server (e.g., no pandoc for saving notebooks as PDFs)
    Miniconda Python 3.x in /opt/conda
    No preinstalled scientific computing packages
    Unprivileged user jovyan (uid=1000, configurable, see options) in group users (gid=100) with ownership 
      over the /home/jovyan and /opt/conda paths
    tini as the container entrypoint and a start-notebook.sh script as the default command
    A start-singleuser.sh script useful for launching containers in JupyterHub
    A start.sh script useful for running alternative commands in the container (e.g. ipython, jupyter kernelgateway,
      jupyter lab)
    Options for a self-signed HTTPS certificate and passwordless sudo
    Pandoc and TeX Live for notebook document conversion
    git, emacs, jed, vim, and unzip
    The R interpreter and base environment
    IRKernel to support R code in Jupyter notebooks
    tidyverse packages, including ggplot2, dplyr, tidyr, readr, purrr, tibble, stringr, lubridate, and broom 
      from conda-forge
    plyr, devtools, shiny, rmarkdown, forecast, rsqlite, reshape2, nycflights13, caret, rcurl,
      and randomforest packages from conda-forge
    pandas, numexpr, matplotlib, scipy, seaborn, scikit-learn, scikit-image, sympy, cython, patsy, statsmodel, 
      cloudpickle, dill, numba, bokeh, sqlalchemy, hdf5, vincent, beautifulsoup, protobuf, and xlrd packages
    ipywidgets for interactive visualizations in Python notebooks
    Facets for visualizing machine learning datasets
    The Julia compiler and base environment
    IJulia to support Julia code in Jupyter notebooks
    HDF5, Gadfly, and RDatasets packages


