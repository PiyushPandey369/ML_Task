# Multiple Linear Regression using Matrix Method and Scikit-Learn

This repository contains the implementation of a Multiple Linear Regression model developed as part of the Internal Evaluation Assignment.

The objective is to predict **Total Internal Marks (out of 50)** using student behavioral indicators and compare the mathematical matrix-based approach with a practical machine learning implementation.

---

## Assignment Overview

The assignment consists of two parts:

### Part A – Manual Calculation (Theory)

A small subset of the dataset containing 6 student records was selected.

Using the top three behavioral indicators, Multiple Linear Regression was manually computed using the **Normal Equation**.

The following steps were performed:

- Correlation Analysis
- Feature Selection
- Data Preprocessing
- Matrix Formation
- Matrix Transpose
- Matrix Multiplication
- Matrix Inversion
- Regression Coefficient Calculation
- Prediction
- Residual Error Calculation

---

### Part B – Practical Implementation

The complete dataset was used to train and evaluate a Multiple Linear Regression model using Python and Scikit-Learn.

The workflow includes:

- Data Loading
- Data Cleaning
- Outlier Handling
- Feature Selection
- Train-Test Split
- Model Training
- Prediction
- Performance Evaluation

Evaluation Metrics:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## Dataset Information

Target Variable:

- `Total_Internal_Marks_50`

Behavioral Indicators Considered:

- Theory Attendance Percentage
- Assignment Scores
- Lab Attendance Percentage
- Lab Reports
- ML on Git
- Viva Marks

Excluded Features:

- `CRN`
- `Final_Theory_Marks_30`
- `Final_Practical_Marks_20`

These columns were excluded because they either act as identifiers or directly contribute to the final internal marks.

---

## Preprocessing Steps

The following preprocessing steps were performed:

- Removal of inactive records containing all-zero values
- Detection and handling of outliers using boxplot analysis
- Missing value inspection
- Data consistency verification
- Feature matrix preparation

---

## Project Structure

```text
ML_Assignment_Part_B/
│
├── README.md
├── LICENSE
│
├── behavioral_indicators_internal_marks.csv
│   └── Original dataset
│
├── subset.csv
│   └── 6-record subset used for manual matrix calculations
│
├── maths_work.ipynb
│   └── Matrix method implementation
│       - Matrix formation
│       - Xᵀ calculation
│       - XᵀX computation
│       - Matrix inverse
│       - Coefficient calculation
│       - Prediction and residual error
│
└── part_B.ipynb
    └── Practical implementation using Scikit-Learn
        - Data preprocessing
        - Correlation analysis
        - Train-test split
        - Model training
        - Prediction
        - Evaluation metrics
```

---

## Technologies Used

- Python
- NumPy
- Pandas
- Scikit-Learn
- Matplotlib
- Jupyter Notebook

---

## Model Performance

The practical implementation was evaluated using:

| Metric | Value |
|----------|----------|
| MAE | 2.325 |
| MSE | 7.816 |
| RMSE | 2.796 |
| R² Score | 0.695 |

The model explains approximately **69.5% of the variance** in student internal marks based on the selected behavioral indicators.

---

## Learning Outcomes

Through this project:

- Understood the mathematical foundation of Multiple Linear Regression.
- Applied the Normal Equation using matrix operations.
- Performed feature selection using correlation analysis.
- Implemented regression models using Scikit-Learn.
- Evaluated model performance using standard regression metrics.
- Compared manual and programmatic approaches to machine learning.

---

## Author

**Piyush Pandey**

Machine Learning Assignment – Multiple Linear Regression using Matrix Method and Scikit-Learn.
