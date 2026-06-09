# Loan Approval Prediction

## Overview

This project was completed as part of my **Data Science Internship at Alfido Tech**. The objective was to build and evaluate machine learning models capable of predicting loan approval status based on applicant information.

The project covers the complete machine learning workflow, including data preprocessing, feature engineering, class imbalance handling, model training, evaluation, and deployment recommendations.

---

## Dataset

**Dataset:** Loan Approval Prediction Case Study

The dataset contains applicant information such as:

* Gender
* Marital Status
* Dependents
* Education
* Self Employment Status
* Applicant Income
* Co-applicant Income
* Loan Amount
* Loan Term
* Credit History
* Property Area
* Loan Status (Target Variable)

### Dataset Summary

* **Records:** 614
* **Features:** 12
* **Target Variable:** Loan Status

---

## Project Objectives

* Clean and preprocess the dataset
* Handle missing values
* Encode categorical variables
* Scale numerical features
* Address class imbalance using SMOTE
* Train and compare multiple machine learning models
* Evaluate model performance using industry-standard metrics
* Provide deployment recommendations

---

## Data Preprocessing

### Missing Value Handling

* Numerical features imputed using median values
* Categorical features imputed using mode values

### Feature Engineering

Created additional features including:

* Total Income
* Loan-to-Income Ratio
* EMI Estimation
* Balance Income

### Class Imbalance Handling

To improve model performance on minority classes:

* Applied **SMOTE (Synthetic Minority Oversampling Technique)** on training data.

---

## Models Evaluated

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Gradient Boosting
5. XGBoost
6. LightGBM

---

## Evaluation Metrics

Models were evaluated using:

* Precision
* Recall
* F1 Score
* ROC-AUC Score

### Best Performing Model

**Random Forest Classifier**

| Metric    | Score |
| --------- | ----- |
| Precision | 0.847 |
| Recall    | 0.847 |
| F1 Score  | 0.847 |
| ROC-AUC   | 0.821 |

---

## Key Insights

* Credit History is the strongest predictor of loan approval.
* Higher applicant income increases approval probability.
* Lower loan burden relative to income improves approval chances.
* EMI burden influences lending decisions significantly.
* Property area and applicant profile contribute to approval outcomes.

---

## Business Interpretation

The model can assist financial institutions by:

* Reducing manual screening effort
* Identifying high-risk applications earlier
* Improving consistency in approval decisions
* Supporting loan officers with data-driven recommendations

---

## Deployment Recommendation

### Recommended Model

**Random Forest Classifier**

### Suggested Threshold

**0.25**

### Reason

* Provides a strong balance between Precision and Recall.
* Achieves the highest F1 Score during threshold optimization.
* Suitable for minimizing missed approvals while maintaining acceptable risk levels.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Imbalanced-Learn (SMOTE)
* XGBoost
* LightGBM
* SHAP
* Matplotlib
* Seaborn

---

## Repository Structure

```text
TASK-2/
│
├── Loan_Approval_Prediction.ipynb
├── Loan_Report.pdf
└── README.md
```

---

## Results

This project demonstrates an end-to-end machine learning pipeline for loan approval prediction, combining:

* Data Cleaning
* Feature Engineering
* Class Imbalance Handling
* Model Comparison
* Explainable AI Techniques
* Deployment Recommendations

The final solution provides actionable insights for lending institutions while maintaining strong predictive performance.

---

## Author

**Bikkavolu Bhuvan**
Data Science Intern
Alfido Tech Internship Program
