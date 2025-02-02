**🚀 Capstone Project: Microsoft - Classifying Cybersecurity Incidents with Machine Learning 🛡️**

# Microsoft - Classification of Cybersecurity Incidents

## Overview
This repository implements a machine learning pipeline for classifying cybersecurity incidents into three categories: True Positive (TP), Benign Positive (BP), and False Positive (FP). The project aims to support Security Operation Centers (SOCs) in automating incident triage through advanced data preprocessing, feature engineering, and classification techniques.

## Key Features

### Extensive Data Preprocessing and Feature Engineering
- Null value handling and removal of irrelevant features
- Time-based feature extraction (day, hour, etc.) from timestamps
- Label encoding for categorical variables
- Feature correlation analysis to drop highly correlated features

### Machine Learning Model Training and Optimization
- Baseline models: Logistic Regression and Decision Trees
- Advanced models: Random Forest, Gradient Boosting and XGBoost
- Techniques to handle class imbalance: resample

### Model Evaluation
- Metrics: Macro-F1 score, precision, recall
- ROC curve analysis for model performance validation
- Confusion matrix for detailed error analysis
- Cross-validation to ensure model robustness

### Deployment-Ready Solution
- Final model saved using joblib for easy deployment
- Demonstrated successful model loading and prediction on test dataset

## Business Use Cases

### 1. Security Operation Centers (SOCs)
- Automate the triage process to prioritize critical threats efficiently
- Model shows 86% accuracy in identifying true positives

### 2. Incident Response Automation
- Enable systems to suggest appropriate actions for incident mitigation
- High precision (90%) for critical incidents

### 3. Threat Intelligence
- Enhance detection capabilities using historical evidence
- Strong discrimination ability with AUC scores > 0.99 for all classes

### 4. Enterprise Security Management
- Reduce false positives and ensure timely addressing of true threats
- 77% accuracy in identifying false positives

## Results

### Best Model: XGBoost with hyperparameter tuning

### Performance Metrics
- Overall Accuracy: 84%
- Macro Average:
  - Precision: 0.85
  - Recall: 0.84
  - F1-score: 0.84

### Class-wise Performance

#### 1. False Positives (Class 0)
- Precision: 0.85
- Recall: 0.77
- F1-score: 0.81

#### 2. Benign Positives (Class 1)
- Precision: 0.78
- Recall: 0.89
- F1-score: 0.83

#### 3. True Positives (Class 2)
- Precision: 0.90
- Recall: 0.86
- F1-score: 0.88

### Model Validation

#### ROC Curve Analysis
- Class 0 AUC: 0.9971
- Class 1 AUC: 0.9946
- Class 2 AUC: 0.9946

#### Confusion Matrix Insights
- Strong classification performance for all classes
- Highest accuracy in identifying Benign Positives (89%)
- Most confusion between False Positives and Benign Positives (17% misclassification)
- Minimal confusion in critical cases (True Positives)

### Deployment Validation
- Successfully deployed using joblib
- Maintained consistent performance on test dataset
- Equal support distribution across classes (902,698 samples per class)
- Robust generalization demonstrated through balanced macro and weighted averages


###📚 **Conclusion**

Through rigorous data preprocessing, feature engineering, and model tuning, we achieved a highly performant XGBoost classifier capable of effectively detecting and categorizing threats. The model demonstrates strong potential for real-world deployment, helping to enhance cybersecurity defense mechanisms in a practical, scalable manner.
