# Credit Card Fraud Detection Using Advanced Classification Algorithms

## Project Overview
This project focuses on building a robust credit card fraud detection model using advanced machine learning classification algorithms. The dataset, obtained from Kaggle, consists of anonymized transaction data with labels indicating whether a transaction is fraudulent or not. The primary goal is to accurately classify transactions as fraudulent or non-fraudulent, with a particular focus on handling the significant class imbalance present in the data.

## Key Objectives
- **Data Preprocessing**: Handle missing values, balance the dataset, and standardize features.
- **Model Evaluation**: Train and evaluate multiple classification models to determine the most effective algorithm.
- **Visualization**: Provide insights through visualizations such as class distribution, confusion matrices, and ROC-AUC curves.

## Dataset
- **Source**: The dataset is publicly available on Kaggle.
- **Features**: The dataset includes 31 columns with anonymized features (V1 to V28), transaction time (`Time`), transaction amount (`Amount`), and the target variable (`Class`).
- **Target Variable**: `Class` - 0 indicates non-fraudulent transactions, and 1 indicates fraudulent transactions.

## Methodology
### 1. Data Preprocessing
- **Missing Values**: The dataset was checked for missing values, and no missing data was found.
- **Class Imbalance**: The dataset was highly imbalanced, with a majority of transactions being non-fraudulent. This imbalance was addressed using SMOTE (Synthetic Minority Over-sampling Technique) to create a balanced dataset.

### 2. Model Selection
Three models were trained and evaluated:
- **XGBoost Classifier**
- **Random Forest Classifier**
- **Neural Network Classifier**

### 3. Model Evaluation
Each model was evaluated based on accuracy, ROC-AUC score, precision, recall, and the confusion matrix. The Random Forest model emerged as the best performer with an accuracy of 99.99%.

## Visualizations and Explanations
### 1. Class Distribution
- The bar plot shows the significant imbalance between non-fraudulent and fraudulent transactions. This imbalance was addressed using SMOTE.

### 2. Confusion Matrix
- The confusion matrix visualizes the performance of the model in correctly classifying fraudulent and non-fraudulent transactions. The Random Forest model demonstrated near-perfect classification with minimal misclassifications.

### 3. ROC-AUC Curve
- The ROC-AUC curve shows the trade-off between the true positive rate and false positive rate. The Random Forest model's curve is close to the top-left corner, indicating high performance.

## Key Insights
- **Balanced Dataset**: Balancing the dataset with SMOTE significantly improved the model's ability to detect fraudulent transactions.
- **Best Model**: The Random Forest classifier was the best-performing model with an accuracy of 99.99% and an outstanding ROC-AUC score.
- **Model Reliability**: The strong performance across all metrics indicates that the model is reliable and can be effectively used to minimize financial losses due to fraudulent transactions.

## Conclusion
This project successfully developed a credit card fraud detection model with high accuracy and reliability. The use of SMOTE for balancing the dataset, combined with the implementation of advanced classification algorithms, resulted in a model that can be deployed in real-world scenarios to detect and prevent fraudulent transactions.
