# Credit Risk Classification

## Project Overview

An end-to-end machine learning workflow for credit risk classification using applicant demographic, financial, and credit-history information.

The project evaluates how preprocessing, feature engineering, feature selection, and hyperparameter tuning affect Random Forest classification performance.

## Approach

- Data preparation and train-test split
- Categorical and numerical feature preprocessing
- Random Forest baseline model
- Feature engineering
- Feature selection using SelectKBest
- Hyperparameter tuning using GridSearchCV
- Final evaluation on unseen test data
- Macro F1 used as the primary evaluation metric

## Feature Engineering

Three additional features were developed:

- **Age** — derived from date of birth
- **AmountPerMonth** — loan amount relative to duration
- **FinancialHistory** — combines previous accounts and previous default history

## Results

| Model Stage | Mean Macro F1 |

| Baseline | 0.5218 |
| Feature Engineering | 0.7591 |
| Feature Selection | 0.7723 |
| Hyperparameter Tuning | 0.7758 |
| Final Unseen Test | **0.7845** |

The final Random Forest model achieved a **Macro F1 score of 0.7845** on the unseen test dataset.

## Technologies

Python · Pandas · NumPy · scikit-learn · Random Forest · SelectKBest · GridSearchCV · Cross-Validation

## Repository Contents

- `Credit-Risk-Classification.ipynb` — complete analysis, code, model development, and evaluation
