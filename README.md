2U
==============================

![](https://media.vanityfair.com/photos/5a332ad62d48cc419d393ee0/master/w_1600%2Cc_limit/kylo-rey-fight.gif)

This project is dockerized for running R and Python within Rnotebooks.

To reporduce notebooks you can follow these steps

### prerequisites

You will need these to run development environment;

- docker
- make

Clone this repo and open a shell in folder.

### Spinup Rstudio

To spinup Rstudio run

```
sudo make dev-init
```

The project folder will be mounted inside the container for ease of use.

### Spinup Jupyter

Jupyter is also available if you prefer

```
sudo make dev-jupyter
```

This command requires the container to be running (from init for example)

Other make commands are available 

```
make help
```

## Results

The results for the submission can be found in `notebooks` along with the rnotebooks.

To view the output open the files ending in .html or open the files endning in Rmd to run/view the code yourself.

Folder layout
------------

    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    |
    ├── README.md          <- The top-level README for developers using this project.
    |
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docker
    │   ├── dev            <- Contains a Dockerfile for the dev environment.
    │   └── prod           <- Contains a Dockerfile for the prod environment.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    |
    ├── 2u                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module.
    │   ├── data           <- Scripts to download or generate data
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   ├── features       <- Scripts to turn raw data into features for modeling    
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations predictions.
    |
    └── tox.ini            <- tox file with settings for running tox; see tox.testrun.org


--------
