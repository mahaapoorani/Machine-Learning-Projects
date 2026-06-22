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
- Hyperparameter Tuning
