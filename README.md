# adv_mla_at2

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

This project focuses on predicting precipitation in Australia using machine learning. Two XGBoost models were developed: a regression model to predict the precipitation sum over the next three days, and a classification model to predict whether it will rain seven days ahead. The models are trained on historical weather data from [Open-Meteo](https://open-meteo.com/en/docs/historical-weather-api).

The API for this project is available at: https://github.com/Shawynot33/adv_mla_at2_api/
The model has been deployed on Render: https://adv-mla-at2-25552249.onrender.com 

## Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         adv_mla_at2 and configuration for tools like black
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
└── adv_mla_at2   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes adv_mla_at2 a Python module
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

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Shawynot33/adv_mla_at2
cd adv_mla_at2
```

2. Install dependencies:

```bash
pip install -rr requirements.txt
```
or if using Poetry:
```bash
poetry install
```

## Additional Information

- **Notebooks:** Jupyter notebooks for data exploration and model development are located in the `notebooks/` folder.  
- **Trained Models:** The saved XGBoost models for regression and classification are located in the `models/` folder.



--------

