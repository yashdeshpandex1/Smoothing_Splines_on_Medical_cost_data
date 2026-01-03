# Splines and Tree-Based Methods on Medical Cost Data

This project explores and compares **classical regression, spline-based models, and modern tree-based ensemble methods** to predict individual medical insurance charges using demographic and lifestyle features.

The goal is to analyze model performance, non-linearity handling, and predictive accuracy using cross-validation and test-set evaluation.

---

## 📊 Dataset

The dataset contains patient-level medical and demographic information with insurance charges as the target variable.

### Features
| Feature | Description |
|-------|------------|
| age | Age of the individual |
| sex | Gender |
| bmi | Body Mass Index |
| children | Number of dependents |
| smoker | Smoking status |
| region | Residential region |
| charges | Medical insurance cost (target) |

---

## 🧠 Models Implemented

The following regression models were trained and evaluated:

- Polynomial Regression  
- Regression Splines  
- Decision Trees  
- Random Forests  
- Gradient Boosting  
- Extreme Gradient Boosting (XGBoost)  
- Bayesian Additive Regression Trees (BART)

These models allow comparison between parametric, semi-parametric, and non-parametric approaches.

---

## 🛠️ Methodology

- Performed data preprocessing including encoding of categorical variables.
- Applied **Cross-Validation** to tune hyperparameters and prevent overfitting.
- Evaluated models using:
  - Mean Squared Error (MSE)
  - R² Score on test data
- Compared bias–variance tradeoffs across different model families.

---

## 📈 Results

- **Best Test MSE:** `16,441,907.34`
- **Best Model:** Extreme Gradient Boosting (XGBoost)
- **Test R²:** `0.8938`

XGBoost significantly outperformed linear, spline-based, and single-tree models, capturing complex interactions and non-linear relationships in the data.

---

## 📦 Requirements

```bash
pip install numpy pandas scikit-learn xgboost matplotlib seaborn
