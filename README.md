🔧 Predictive Maintenance Using Machine Learning
📌 Project Overview

This project focuses on building an end-to-end predictive maintenance system to identify machine failures and failure types using manufacturing process data. The goal is to proactively detect failures and reduce unplanned downtime by leveraging machine learning techniques.

🧠 Problem Statement

Machine failures are rare but costly events in manufacturing. Traditional maintenance strategies often fail to detect early warning signs. This project aims to build a failure-focused ML model that prioritizes early detection over overall accuracy.

📊 Dataset Overview

Industrial machine sensor and process data

Binary target variable: Machine failure (Yes/No)

Multiple failure subtypes

Highly imbalanced dataset

🔍 Project Workflow

Data Understanding & EDA

Structured visualization using UBM approach

Failure distribution analysis

Feature relationship exploration

Data Wrangling

Removal of identifier columns

Consolidation of failure types

Verification of missing and duplicate values

Feature Engineering & Selection

Log transformations for skewed variables

Feature creation based on domain knowledge

Multicollinearity handling using VIF

Interpretability preserved without PCA

Data Scaling

Standard Scaling for numerical features

Handling Class Imbalance

SMOTE applied only on training data

Prevents data leakage and improves recall

Model Development

Logistic Regression (Baseline)

Random Forest

Gradient Boosting Classifier

Model Evaluation

Metrics: Recall, F1 Score, ROC AUC

Business-focused evaluation strategy

Hyperparameter Tuning

GridSearchCV and RandomizedSearchCV

Balanced against computational constraints

Model Explainability

SHAP used for global feature importance

Key drivers identified: power usage, tool wear, temperature deviation

🏆 Final Model Selection

The Gradient Boosting Classifier (baseline version) was selected as the final model due to:

Highest recall for failure detection

Strong ROC AUC

Better alignment with business objectives

📈 Business Impact

Early failure detection

Reduced unplanned downtime

Preventive maintenance optimization

Improved operational reliability

🛠️ Tech Stack

Python

Pandas, NumPy

Scikit-learn

Imbalanced-learn (SMOTE)

SHAP

Matplotlib, Seaborn

🚀 Future Improvements

Threshold tuning for precision–recall trade-off

Real-time model deployment

Cost-sensitive learning

Monitoring model drift in production

📬 Contact

If you have suggestions or want to collaborate, feel free to open an issue or reach out.
