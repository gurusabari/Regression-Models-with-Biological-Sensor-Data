# Health Prediction Model

## Overview

This model aims to predict the current health of an organism based on measurements from two biological sensors measuring their bio-markers. The target variable represents the current health status, with negative values indicating that it is lesser than the average case. The task involves training linear regression and support vector regression (SVR) models on the training data and evaluating their performance on the test data using mean squared error (MSE) and mean absolute error (MAE) metrics.

## Dataset

The dataset consists of two files:
- `p1_train.csv`: Training data containing features and the target variable.
- `p1_test.csv`: Test data containing features and the target variable.

The last column in both datasets represents the target variable (current health).

## Models Used

Two models are employed for this task:
1. **Linear Regression**: A basic linear regression model is used for predicting the target variable based on the features.
2. **Support Vector Regression (SVR)**: SVR model with a linear kernel is utilized to predict the target variable.

## Workflow

1. **Data Preprocessing**:
    - The training and test datasets are loaded using Pandas.
    - Features and target variables are extracted from the datasets.
    - Standard scaling is applied to the features using `StandardScaler` from scikit-learn.

2. **Model Training**:
    - Linear regression model is trained on the scaled training data.
    - SVR model with a linear kernel is trained on the scaled training data.

3. **Evaluation**:
    - Predictions are made using the trained models on the test data.
    - MSE and MAE are calculated for both linear regression and SVR models.
    - Evaluation metrics are reported for comparison.

## Usage

To use this model:
1. Ensure that Python and required libraries (Pandas, scikit-learn) are installed.
2. Download the dataset files `p1_train.csv` and `p1_test.csv`.
3. Run the provided Python script (`Regression_Problem.ipynb`) to train the models and evaluate their performance.

## Files

- `Regression_Problem.ipynb`: Python script containing the implementation of the model.
- `p1_train.csv`: Training dataset.
- `p1_test.csv`: Test dataset.

## Dependencies

- Python 3.x
- Pandas
- scikit-learn

## Author

Guru Sabari S
