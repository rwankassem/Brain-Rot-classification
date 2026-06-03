# Teen Phone Addiction Analysis

This repository contains a self-contained machine learning analysis of a teen phone addiction dataset.
The main work is done in `Brain rot.ipynb`, which loads the dataset, performs data quality checks, preprocesses categorical data, trains regression models, and compares performance.

## Repository Contents

- `Brain rot.ipynb` - Jupyter Notebook with the full end-to-end analysis.
- `teen_phone_addiction_dataset.csv` - Dataset used in the notebook.
- `best_model.joblib` / `best_model.pkl` - Serialized final trained model artifact.
- `label_encoders.joblib` / `label_encoders.pkl` - Serialized label encoders for categorical preprocessing.
- `scaler.joblib` / `scaler.pkl` - Serialized scaler used for feature normalization.

## Project Overview

The notebook explores teen phone addiction behavior and builds predictive models for the addiction level.
The analysis includes:

- dataset overview and validation
- categorical feature encoding comparisons
- exploratory data analysis (EDA) and feature correlations
- train-test splitting and scaling
- training multiple regression models
- evaluating models with R², RMSE, and MAE
- visualization of model performance

## Dataset Summary

The dataset contains information about teenagers and their phone usage, including:

- demographics: age, gender, location, school grade
- phone usage patterns: daily usage hours, phone checks, app usage, weekend usage
- screen use content: social media, gaming, education, bedtime screen time
- health metrics: sleep, anxiety, depression, self-esteem
- behavioral factors: academic performance, exercise, parental control, family communication
- target: addiction level on a numerical scale

## How to Use

1. Open `Brain rot.ipynb` in Jupyter Notebook or JupyterLab.
2. Ensure `teen_phone_addiction_dataset.csv` is accessible at the notebook path.
3. Install required Python packages.
4. Run cells sequentially from top to bottom.


## Notes

- The notebook performs categorical encoding using both label encoding and one-hot encoding.
- It standardizes features before training regression models.
- Model artifacts are saved to allow future prediction or deployment without re-training.

## Artifact Usage

- `best_model.joblib` / `best_model.pkl` can be loaded with `joblib.load()` or `pickle.load()`.
- `scaler.joblib` / `scaler.pkl` should be used to scale new feature data before prediction.
- `label_encoders.joblib` / `label_encoders.pkl` should be used to transform categorical inputs consistently.

## Contact

For questions or updates, open the notebook and inspect the analysis sections directly.
