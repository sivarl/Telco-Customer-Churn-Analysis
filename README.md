# Telco Customer Churn Prediction

## Objective
The goal of this project is to analyze customer behavior and build a machine learning model to predict churn.

---

## Project Workflow
1. Data Loading and Understanding
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Model Training (Logistic Regression)

---

## Key Insights
- Customers with higher monthly charges show higher churn
- Long-term contracts reduce churn
- Customers using more services tend to stay longer
- Electronic check users have higher churn probability

---

## Model Details
- Model: Logistic Regression
- Evaluation Metric: ROC-AUC, Recall

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-Learn

---

## Project Structure
'''
data/
└── processed/
├── telco_churn_cleaned.csv
└── telco_churn_features.csv

notebooks/
├── 01_data_loading_and_understanding.ipynb
├── 02_data_cleaning.ipynb
├── 03_exploratory_data_analysis.ipynb
├── 04_feature_engineering.ipynb
└── 05_model_training.ipynb
'''

---

## Future Improvements
- Experiment with advanced models such as Random Forest and Gradient Boosting to improve performance
- Perform hyperparameter tuning to optimize model performance
- Improve recall for churn prediction by handling class imbalance more effectively
- Explore deployment options using Flask or FastAPI for real-time predictions
