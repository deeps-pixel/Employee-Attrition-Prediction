# Employee Attrition Prediction

## Project Overview
This project develops a **Logistic Regression** model to predict employee attrition using a dataset of 3,500 records. The analysis was conducted under a strict "no-regularization" constraint.

### Key Highlights
- **Class Imbalance:** Handled a severe 1.97% attrition rate using balanced class weighting.
- **Feature Engineering:** Expanded 14 numerical features into **679 polynomial and interaction terms** (degree 3).
- **Optimization:** Used a constrained forward selection to find 10 key interaction features.
- **Threshold Tuning:** Optimized the classification threshold to maximize Recall while keeping the **False Positive Rate below 5%**.

## Model Performance
- **Recall:** 23.2% (Identifies ~1 in 4 actual leavers)
- **False Positive Rate:** 3.3%
- **OOF AUC-ROC:** 0.61
- **Kaggle Score:** 0.94266

## Key EDA Insights
- **Overtime:** Employees working overtime are twice as likely to quit.
- **Age:** High risk found in younger (mid-20s) and older (50+) employees, with stability in the 35-45 range.
- **Stagnation:** Employees waiting over 7 years for a promotion show a significant increase in flight risk.

## Repository Contents
- `s16751_Assignment1_DS.ipynb`: The complete analysis and modeling notebook.
- `s16751_Assignment1_DS.pdf`: The technical report version of the project.
- `.gitignore`: Excludes large datasets and local artifacts.

## Technology Stack
- Python (Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Statsmodels)
