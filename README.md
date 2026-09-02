# From Theory to Implementation: Data Preprocessing & Feature Selection

## Loan Prediction Dataset

### Course
Machine Learning

### Assignment Type
Group Practical Assignment

## Group Member

- **Aayushi Sonkar** — CSJMA23001390001,
- **Aryan Kumar** — CSJMA23001390011,
- **Sahil Kumar Yadav** — CSJMA23001390038,
- **Shubhash Verma**— CSJMA23001390042

## Project Overview

This project focuses on applying important Data Preprocessing and Feature Selection techniques to a Loan Prediction Dataset.

The objective is to understand the dataset, clean and preprocess the data, transform categorical and numerical features, detect outliers, perform feature scaling, and select useful features for a machine learning classification problem.

## Problem Statement

The dataset represents a loan approval problem. The objective is to analyze applicant information and determine whether a loan application is likely to be approved or rejected.

### Target Variable

`Loan_Status`

- `Y` → Loan Approved
- `N` → Loan Not Approved

### Problem Type

Binary Classification

## Dataset

The dataset contains **614 records and 13 columns**.

### Features

- Loan_ID
- Gender
- Married
- Dependents
- Education
- Self_Employed
- ApplicantIncome
- CoapplicantIncome
- LoanAmount
- Loan_Amount_Term
- Credit_History
- Property_Area
- Loan_Status

## Techniques Implemented

### Data Exploration
- Dataset shape and structure
- Data types
- Missing value analysis
- Unique value analysis
- Basic statistics

### Statistics From Scratch
- Mean
- Median
- Mode
- Variance
- Standard Deviation
- Range

### Data Cleaning
- Missing value treatment
- Duplicate detection
- Categorical data validation
- Numerical data validation

### Encoding
- Label Encoding from scratch
- One-Hot Encoding from scratch

### Outlier Detection
- IQR method
- Z-score method
- IQR vs Z-score comparison

### Data Transformation
- Log transformation
- Skewness analysis

### Feature Scaling
- Min-Max Normalization
- Standardization
- Training-data-based scaling to reduce data leakage

### Visualization
- Histograms
- Box plots
- Bar charts
- Scatter plots
- Correlation analysis

### Feature Selection
- Variance Threshold
- Pearson Correlation
- Chi-Square Test
- ANOVA F-Test
- Mutual Information
- Comparison of feature-selection techniques
- Leakage-safe feature selection

## Final Feature Selection

### Selected Features

1. Married
2. Dependents
3. Education
4. ApplicantIncome
5. CoapplicantIncome
6. LoanAmount
7. Loan_Amount_Term
8. Credit_History
9. Property_Area

### Removed Features

- Gender
- Self_Employed

After encoding categorical features, the final ML-ready dataset contains **14 input features + 1 target column**.

## Final Dataset

| Dataset | Rows | Columns |
|---|---:|---:|
| Original Dataset | 614 | 13 |
| Training Dataset | 491 | 15 |
| Testing Dataset | 123 | 15 |

The final training and testing datasets contain **no missing values** and **no duplicate records**.

The numerical features `ApplicantIncome`, `CoapplicantIncome`, and `LoanAmount` were standardized using parameters learned from the training data.

## From-Scratch Implementation

The major preprocessing and feature-selection calculations were implemented using basic Python logic before library-based verification.

Library functions were used where appropriate to verify the manually calculated results.

## Files in This Repository

- `loan prediction colab .ipynb` — Complete Google Colab notebook containing the implementation, outputs, visualizations, and interpretations.
- `loan_prediction.csv` — Loan Prediction Dataset.

## How to Run

1. Download or clone this repository.
2. Open the `.ipynb` file using Google Colab or Jupyter Notebook.
3. Make sure `loan_prediction.csv` is available in the same working environment.
4. Run the notebook from the first cell to the last cell.

## Conclusion

The project demonstrates a complete workflow for Data Preprocessing and Feature Selection, including manual implementation of important statistical and machine learning techniques.

The final dataset is prepared for machine learning use after cleaning, encoding, transformation, feature selection, and training-data-based feature scaling.
