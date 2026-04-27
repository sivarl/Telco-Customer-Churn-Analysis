# Telco Customer Churn Prediction

## Objective
The goal of this project is to analyze customer behavior and build a machine learning model to predict churn.

---

## Business Problem
Customer churn is a critical challenge for telecom companies, as acquiring new customers is more expensive than retaining existing ones. This project focuses on identifying customers who are likely to churn, enabling the business to take proactive retention actions and reduce revenue loss.

---

## Project Workflow
1. Data Loading and Understanding
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Model Training (Logistic Regression)

---

## Key Insights
- Customers with higher monthly charges are more likely to churn
- Long-term contracts significantly reduce churn probability
- Customers using multiple services tend to have higher retention
- Customers using electronic check payments show higher churn risk

---

## Model Development & Evaluation
Evaluation Metric: ROC-AUC, Recall
1. Logistic Regression
- Threshold Optimization: Adjusted classification threshold to improve recall and better identify potential churn customers
- Handling Class Imbalance: Applied class_weight in Logistic Regression to address imbalance and improve model sensitivity towards churn class, resulting in higher recall and reduced false negatives

2. Decision Tree
- Observed overfitting in the baseline model (very high training accuracy, low test performance)
- Applied hyperparameter tuning (max_depth, min_samples_leaf) to control overfitting

### Model Comparison
- Logistic regression and decision tree achieved similar ROC-AUC (~0.84)
- Logistic regression provided significantly higher recall(0.88)
- Decision tree captured non-linear patterns but missed more churn customers

Logistic Regression model was selected as the final model due to its higher recall and better suitability for churn prediction, where identifying at-risk customers is critical.

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-Learn

---

## Project Structure
```
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
```

---

## Future Improvements
- Experiment with advanced models such as Random Forest and Gradient Boosting to improve performance
- Perform hyperparameter tuning to optimize model performance
- Improve recall for churn prediction by handling class imbalance more effectively
- Explore deployment options using Flask or FastAPI for real-time predictions

---

## Business Impact
The insights from this project can help businesses design targeted retention strategies, such as offering incentives to high-risk customers and promoting long-term contracts to reduce churn.
