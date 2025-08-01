# Job Salary Prediction Using Machine Learning

This project aims to predict salaries for data-related job roles based on features like job title, experience level, company size, remote ratio, and more. Using a dataset from Kaggle, I explore the underlying patterns and train regression models to estimate compensation.

## Dataset
The dataset contains job postings with attributes including:
- Work year, experience level, and employment type
- Job title and remote work ratio
- Company location and size
- Salary (in USD, standardized)

Source: https://www.kaggle.com/datasets/adilshamim8/salaries-for-data-science-jobs

## EDA Highlights
- Most roles are remote-friendly and hybrid roles have the least frequency.
- The biggest salaries are paid in the US. A large percentage of salaries are paid in the US Dollar.
- Salaries are right-skewed; standardization was applied.

## Models Trained
Two regression models were trained and compared:
- **Ridge Regression**
- **Random Forest Regressor**

GridSearchCV was used for hyperparameter tuning with multi-metric scoring (`RMSE` and `R²`).  
**Random Forest** performed best on both metrics.

## 📈 Best Model Performance
| Metric | Value |
|--------|-------|
| RMSE   | *40,680.54* |
| R²     | *0.59* |


## Tech Stack
- Python, Jupyter Notebook  
- `scikit-learn`, `pandas`, `matplotlib`, `seaborn`, `numpy`

## Future Improvements
- Try gradient boosting models (e.g. XGBoost)  
- Deploy a web app for live predictions (Streamlit)