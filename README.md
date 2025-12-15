# Data Analytics in Motorsport: Predicting Formula 1 Race Outcomes

This repository contains the Python code used for my dissertation titled **"Data Analytics in Motorsport: Predicting Formula 1 Race Outcomes."**

The aim of the project is to analyze historical Formula 1 data and apply machine learning methods to:
- predict whether a driver finishes inside the Top 10 (classification), and
- predict the exact finishing position of a driver (regression).

The analysis follows the same structure as the dissertation, including data collection, preprocessing, exploratory analysis, modelling, evaluation and interpretation.

## Repository contents
- 'Data_Analytics_in_Motorsport_Predicting_Formula_1_Race_Outcomes.ipynb'
  This notebook contains the complete analysis pipeline:
  - data download and merging,
  - feature engineering,
  - exploratory data analysis,
  - baseline and advanced models,
  - evaluation metrics,
  - feature importance and SHAP analysis.

All results presented in the dissertation are generated from this notebook.

## Dataset

The project uses the Kaggle dataset **"Formula 1 World Championship (1950-2024)"**.

The dataset includes information about races, drivers, constructors, qualifying, sprint races and pit stops.
The notebook downloads the data using `kagglehub`.

## How to reproduce the results

1. Open the notebook in Google Colab.
2. Run the cells sequentially from top to bottom.
3. Required libraries are installed automatically if missing.
4. The dataset is download within the notebook.

## Methods used

The notebook includes:
- baseline models: Logistic Regression and Linear Regression,
- advanced models: Random Forest and Gradient Boosting,
- evaluation metrics for classification and regression,
- model interpretation using feature importance and SHAP values.

Random states are fixed where possible to improve reproducibility.

## Notes

- Results may vary slightly due to randomness in model training.
- The notebook is intended to support the dissertation and is not designed as a standalone software package.

## Author

Giorgi Chachava
