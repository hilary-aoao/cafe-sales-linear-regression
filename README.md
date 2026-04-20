# Café Sales — Linear Regression Model

## Overview
This project builds a Linear Regression model to predict 
Total Spent per transaction in a café sales dataset. 
It is the second part of my café sales data science project, 
following the data cleaning phase.

## Dataset
- **Source:** Kaggle — Dirty Café Sales Dataset (cleaned version)
- **Rows:** 9,517 transactions
- **Target Variable:** Total Spent

## Project Pipeline

| Step | Description |
|------|-------------|
| Data Loading | Load cleaned café sales CSV |
| Exploration | Understand data structure and types |
| Encoding | One Hot Encode categorical columns |
| Feature Selection | Define X (features) and y (target) |
| Train/Test Split | 80% training, 20% testing |
| Feature Scaling | RobustScaler on numerical columns |
| Model Training | Linear Regression |
| Evaluation | R² Score and MAE |

## Results

| Metric | Score |
|--------|-------|
| R² Score | 0.91 |
| MAE | 1.21 |

The model explains **91% of the variance** in Total Spent 
with an average prediction error of **1.21**.

The high R² score is expected because Total Spent has a 
near perfect linear relationship with Quantity and 
Price Per Unit (Total Spent ≈ Quantity × Price Per Unit).

## Features Used

| Feature | Type | Encoding |
|---------|------|----------|
| Quantity | Numerical | RobustScaler |
| Price Per Unit | Numerical | RobustScaler |
| Month | Numerical | None |
| Payment Method | Categorical | One Hot Encoding |
| Location | Categorical | One Hot Encoding |
| Item | Categorical | One Hot Encoding |

## Tools Used
- Python
- Pandas
- Numpy
- Scikit-learn
- Matplotlib

## Related Projects
- [Café Sales Data Cleaning](https://github.com/hilary-aoao/cafe-sales-data-cleaning)

## About Me
I am currently enrolled in an AI Engineering and Machine 
Learning program, building my skills in data science 
one project at a time.
