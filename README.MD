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
- Most roles are remote-friendly and concentrated in the US.
- Seniority and company size heavily influence compensation.
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
| RMSE   | *41,054.24* |
| R²     | *0.583* |


## Tech Stack
- Python, Jupyter Notebook  
- `scikit-learn`, `pandas`, `matplotlib`, `seaborn`

## Future Improvements
 
- Try ensembling and boosting models (e.g., XGBoost)  
- Deploy a web app for live predictions