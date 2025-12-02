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

# Code Structure
The dataset can be found in the data folder. 
The notebooks can be found in the notebook folder. There should be 3:

1. notebooks/exploratory_data_analysis.ipynb - exploratory data analysis of dataset
2. notebooks/regression_xgboost.ipynb - xgboost regression model
3. notebooks/xgboost_classification_shap.ipynb xgboost classification model + shap analysis
