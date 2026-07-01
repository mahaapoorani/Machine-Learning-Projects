# Machine Learning Projects

## 1. Linear Regression

### California Housing Price Prediction

- Built using Scikit-Learn
- Evaluated using MAE and R² Score
- Learned train-test split and model evaluation

---

## 2. Decision Tree Regression

### California Housing Price Prediction

- Implemented DecisionTreeRegressor
- Explored overfitting and underfitting
- Tuned max_depth parameter

### Results

| Max Depth | Train R² | Test R² |
|------------|-----------|-----------|
| 3 | 0.57 | 0.55 |
| 5 | 0.64 | 0.61 |
| 10 | 0.82 | 0.71 |
| 12 | 0.89 | 0.69 |
| None | 1.00 | 0.63 |

Best Model:
- max_depth = 10
- Test R² = 0.71
- MAE ≈ 40,708

## 3. Random Forest Regression

### California Housing Price Prediction

Random Forest Regression was implemented and compared against Linear Regression and Decision Tree Regression.

### Hyperparameter Tuning

| n_estimators | Test R² | MAE |
|-------------|----------|---------|
| 10 | 0.800 | 33291 |
| 50 | 0.816 | 31990 |
| 100 | 0.817 | 31668 |
| 200 | 0.818 | 31522 |

### Best Model

- n_estimators = 200
- Train R² = 0.976
- Test R² = 0.818
- MAE = 31522

### Key Learnings

- Ensemble Learning
- Bagging
- Random Forest Regression
- Hyperparameter Tuning
- Diminishing Returns
### Key Learnings

- Decision Trees
- Overfitting
- Underfitting
  
## 4. Ridge Regression

### Project Overview

This project demonstrates **Ridge Regression** on the California Housing Prices dataset. Ridge Regression is a regularized version of Linear Regression that helps reduce overfitting by adding an **L2 penalty** to the model's loss function.

---

### Dataset

* **Dataset:** California Housing Prices
* **Target Variable:** `median_house_value`

---

### Data Preprocessing

The following preprocessing steps were performed before training the model:

* Loaded the California Housing dataset.
* Checked dataset information and data types.
* Identified missing values.
* Filled missing values in `total_bedrooms` using the median.
* Applied One-Hot Encoding to the categorical feature (`ocean_proximity`).
* Split the dataset into training and testing sets.
* Standardized numerical features using `StandardScaler`.

---

### Model

Algorithm Used:

* Ridge Regression

Hyperparameter:

* `alpha = 0.01`
* `alpha = 0.1`
* `alpha = 1`
* `alpha = 10`
* `alpha = 100`

---

### Model Performance

| Metric   |     Value |
| -------- | --------: |
| Train R² |    0.6497 |
| Test R²  |    0.6272 |
| MAE      | 50,510.98 |

Best result obtained with:

* **Alpha = 100**

---

### Alpha Comparison

|      Alpha |     Train R² |      Test R² |           MAE |
| ---------: | -----------: | -----------: | ------------: |
|       0.01 |     0.649665 |     0.625424 |     50,670.71 |
|       0.10 |     0.649665 |     0.625427 |     50,670.48 |
|       1.00 |     0.649665 |     0.625457 |     50,668.12 |
|      10.00 |     0.649658 |     0.625736 |     50,646.17 |
| **100.00** | **0.649153** | **0.627228** | **50,510.98** |

---

### Key Learnings

* Ridge Regression is an extension of Linear Regression.
* Ridge uses **L2 Regularization** to reduce overfitting.
* The `alpha` parameter controls the strength of regularization.
* Feature scaling is important before applying Ridge Regression.
* Increasing `alpha` increases regularization strength.
* Very large `alpha` values can lead to underfitting.
* Ridge performs well when features are highly correlated (multicollinearity).

## Cross Validation

### Objective

Evaluate model performance more reliably using multiple train-test splits.

### Concepts Learned

K-Fold Cross Validation
Average Validation Score
Standard Deviation
Model Stability
Generalization

### Best Result

Average Cross Validation R²: 0.824
Standard Deviation: 0.0096

## GridSearchCV

### Objective

Automatically identify the best hyperparameter combination using exhaustive search.

### Concepts Learned

Hyperparameter Tuning
Parameter Grid
Cross Validation
Best Parameters
Best Estimator
Best Cross Validation Score

### Hyperparameters Tuned

n_estimators
max_depth
min_samples_split

## RandomizedSearchCV

### Objective

Perform efficient hyperparameter tuning by randomly sampling parameter combinations.

### Concepts Learned

Randomized Hyperparameter Search
n_iter
Faster Optimization
Trade-off Between Speed and Accuracy

Best Hyperparameters Found

{
    'n_estimators': 300,
    'max_depth': 20,
    'min_samples_split': 5
}

Performance

Cross Validation R²: 0.8187
Test R²: 0.8186
MAE: 31,548


## Machine Learning Concepts Covered
- Regression Algorithms
- Linear Regression
- Decision Tree Regression
- Random Forest Regression
- Ridge Regression
- Model Evaluation
- Train/Test Split
- MAE (Mean Absolute Error)
- R² Score
- Actual vs Predicted Analysis
- Feature Engineering
- Missing Value Imputation
- One-Hot Encoding
- Feature Scaling
- Feature Importance
- Model Validation
- K-Fold Cross Validation
- Model Stability Analysis
- Hyperparameter Tuning
- Manual Hyperparameter Tuning
- GridSearchCV
- RandomizedSearchCV
- Learning Outcomes

## 🎯 Learning Outcomes

Through these projects, I gained hands-on experience in:

- Data preprocessing (handling missing values and one-hot encoding)
- Splitting data into training and testing sets
- Building regression models using Scikit-learn
- Understanding Linear Regression, Decision Tree Regression, Random Forest Regression, and Ridge Regression
- Evaluating models using MAE and R² Score
- Identifying and reducing overfitting and underfitting
- Performing feature engineering and feature importance analysis
- Applying feature scaling for regularized models
- Using K-Fold Cross Validation to measure model generalization
- Performing manual hyperparameter tuning
- Optimizing models using GridSearchCV and RandomizedSearchCV
- Comparing multiple machine learning algorithms on the same dataset
- Interpreting model predictions and evaluation metrics
- Writing clean, structured, and reproducible machine learning code

## 📚 Skills Developed

- Python
- NumPy
- Pandas
- Scikit-learn
- Machine Learning
- Data Preprocessing
- Feature Engineering
- Model Evaluation
- Hyperparameter Tuning
- Cross Validation
- Ensemble Learning
- Regression Analysis

# Logistic Regression - Breast Cancer Classification

## Overview
Implemented **Logistic Regression** on the **Breast Cancer Wisconsin Dataset** to classify tumors as **Malignant** or **Benign**.

## Dataset
- Source: Scikit-learn Breast Cancer Dataset
- Samples: 569
- Features: 30
- Classes:
  - 0 → Malignant
  - 1 → Benign

## Workflow
- Data Loading
- Data Exploration
- Train-Test Split
- Feature Scaling (StandardScaler)
- Logistic Regression Model
- Model Evaluation

## Model Performance
- Accuracy: **97.37%**
- Confusion Matrix:
  ```
  [[41  2]
   [ 1 70]]
  ```
- Evaluated using:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - ROC Curve
  - AUC Score

## Key Learnings
- Binary Classification
- Logistic Regression
- Sigmoid Function
- Feature Scaling
- Confusion Matrix
- Precision, Recall & F1-Score
- ROC Curve & AUC
- Classification Model Evaluation

## Tech Stack
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
