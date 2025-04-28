# Bank Customer Churn Prediction

## Overview

This repository contains a machine learning pipeline for predicting bank customer churn. I explored several classification models, including Logistic Regression, K-Nearest Neighbors, Support Vector Machine, Decision Trees, and Random Forest.

## Dataset Source: 
The dataset was obtained from kaggle. https://www.kaggle.com/datasets/shubhammeshram579/bank-customer-churn-prediction

### Key features:
* **Numerical**: CreditScore, Age, Tenure, Balance, NumOfProducts, EstimatedSalary
* **Categorical**: Geography, Gender
* **Target**: Exited (binary: 0 for "not exited", 1 for "exited")

## Model Performance

| Model                  | Accuracy | Precision | Recall | F1 Score |
| ---------------------- | -------- | --------- | ------ | -------- |
| Logistic Regression    | 0.811    | 0.573     | 0.226  | 0.322    |
| K-Nearest Neighbors    | 0.833    | 0.645     | 0.427  | 0.514    |
| Support Vector Machine | 0.859    | 0.836     | 0.394  | 0.535    |
| Decision Tree          | 0.792    | 0.500     | 0.500  | 0.500    |
| Random Forest          | 0.858    | 0.746     | 0.477  | 0.582    |

## Insights & Key Findings

**Top Performing Models:**

Support Vector Machine achieved the highest accuracy (85.87%).

Random Forest closely followed with 85.77% accuracy.

K-Nearest Neighbors also performed well, better than Logistic Regression and Decision Tree models.

* Key features influencing churn include Age, Balance, and NumOfProducts.

**Challenge:**

There is a  class imbalance in the target variable with significantly more non-churned customers, making recall and F1-score critical metrics in addition to accuracy.


## Future Work

* **Additional ensemble models:** Evaluate XGBoost and LightGBM.
* **Feature engineering:** Explore additional relevant features.
* **Robust validation:** Implement k-fold cross-validation.
* **Pipeline & deployment:** Wrap the preprocessing and final estimator into a scikit-learn Pipeline.
