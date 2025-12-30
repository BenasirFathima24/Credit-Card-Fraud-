# Credit-Card-Fraud-Detection
Credit Card Fraud Detection Pipeline
This project implements a machine learning pipeline to identify fraudulent credit card transactions using the  Credit Card Fraud Detection dataset. It addresses the extreme class imbalance (0.17% fraud) using synthetic oversampling.
🚀 Key Features
Handling Imbalance: Utilizes SMOTE (Synthetic Minority Over-sampling Technique) to balance training data.
Models Implemented:
Logistic Regression: Serves as a baseline statistical model.
XGBoost Classifier: A gradient-boosted decision tree model optimized with L1/L2 regularization to prevent overfitting.
Evaluation Metrics: Focuses on Recall, Precision, and F1-Score rather than simple accuracy to ensure fraud is captured.
Visual Analysis: Includes correlation heatmaps, transaction time distribution plots, and outlier detection boxplots.
🛠️ Requirements
To run this notebook, ensure you have the following libraries installed:
bash
pip install pandas seaborn matplotlib plotly scikit-learn xgboost imbalanced-learn
Use code with caution.
📋 Pipeline Workflow
Data Cleaning: Checks for missing values and removes duplicate records.
EDA: Analyzes the distribution of Time and Amount across fraud vs. non-fraud classes.
Data Splitting: Uses stratify=y during the train-test split to maintain class proportions in both sets.
Resampling: Applies SMOTE only to the training set to prevent data leakage.
Model Training:
Trains a Logistic Regression model.
Trains an XGBoost model with specific hyperparameters (subsample, colsample_bytree) for robustness.
Validation: Employs Stratified K-Fold Cross-Validation to ensure the model generalizes well across different data subsets.
📊 Results & Evaluation
The pipeline outputs:
Confusion Matrix: To visualize False Positives vs. False Negatives.
Recall Score: Critical for fraud detection (minimizing missed fraud).
Classification Report: Providing a detailed breakdown of performance per class.
🔗 Useful Documentation
Imbalanced-Learn SMOTE Documentation
XGBoost Python API Reference
Scikit-learn Classification Metrics
👩 ## Author
Benasir Fathima A
Cultus intership project-2025


