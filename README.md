# Insurance Fraud Detection
This project aims to develop a machine learning model to identify fraudulent claims in insurance data. The goal is to minimize false negatives to ensure that fraudulent claims are detected and flagged effectively.

# Dataset
Target Variable: FraudFound_P (indicates whether a claim is fraudulent).

Features: Includes numerical, categorical, and boolean columns such as Age, VehiclePrice, PolicyType, and Claim Details.

# Data Preprocessing
Label encoding for boolean columns and feature engineering.

SMOTE used to balance the dataset due to class imbalance.

Recursive Feature Elimination with Cross-Validation (RFECV) was used for feature selection.

# Modeling
Algorithms explored: RandomForest, GradientBoosting, BalancedRandomForest, SVC, and LightGBM.

Hyperparameter tuning using Optuna to optimize models.

Pipeline includes encoding, scaling, SMOTE, feature selection, and model training.

# Results
Best Model achieved:

Accuracy: 74.60%

Precision: 13.91%

Recall: 60.34%

F1 Score: 22.61%

ROC AUC Score: 76.07%

# Key Insights
High recall indicates good capture of fraudulent claims, while low precision shows many false positives.

False negatives are prioritized, as missing fraudulent claims can lead to significant financial loss.

# Future Directions
Enhance feature engineering with domain-specific data.

Explore deep learning models or advanced tree-based models (e.g., CatBoost).

Deploy the model for real-time fraud detection and periodic retraining.

