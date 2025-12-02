# Air Quality Prediction Project

Predicting AQI categories (Safe, Caution, Unsafe) and next-day AQI using pollutants and meteorological data.

# Environment Setup

## Create a virtual environment

python3 -m venv .venv

## Activate it

macOS / Linux:
source .venv/bin/activate

Windows (PowerShell):
.venv\Scripts\activate

## Install required dependencies

pip install -r requirements.txt


# Running the Project

## Open Jupyter

jupyter notebook

# Project Structure
- data/
  - aqi_data_labeled.csv         (labeled Safe / Caution / Unsafe)

- notebooks/
  - exploratory_data_analysis.ipynb
  - regression_xgboost.ipynb
  - xgboost_classification_shap.ipynb

- requirements.txt
- README.md
- .gitignore


# Notebooks

1. exploratory_data_analysis.ipynb

Loads and examines the dataset
Performs time-series visualization
Checks pollutant distributions and correlations
Identifies class imbalance

2. regression_xgboost.ipynb

Predicts next-day AQI value using XGBoost Regressor
Includes time-aware train/test split (2021–2022 train, 2023 test)
Evaluates performance (R², RMSE, MAE)
Helps understand pollutant combinations contributing to AQI levels

3. xgboost_classification_shap.ipynb

Hyperparameter-tuned XGBoost classifier
Handles class imbalance using sample weights
Predicts AQI category (Safe, Caution, Unsafe)
Performs SHAP analysis for interpretability
Includes both global (summary plot) and local (waterfall) explanations
