# Heart Attack Prediction using Machine Learning

## Project Overview
This project focuses on analyzing medical health data and building machine learning
models to predict whether a patient is likely to have a heart attack.
The aim is to understand important health indicators and evaluate different models
for accurate prediction.

## Dataset
The dataset contains **1319 patient records** with the following features:
- Age  
- Gender  
- Heart rate  
- Systolic blood pressure  
- Diastolic blood pressure  
- Blood sugar  
- CK-MB  
- Troponin  
- Result (target variable: positive / negative)

The dataset is clean and does not contain missing values.

## Exploratory Data Analysis (EDA)
- Reviewed data structure, shape, and summary statistics
- Analyzed relationships between health parameters using correlation heatmaps
- Observed strong correlation between systolic and diastolic blood pressure
- Cardiac markers like **Troponin** and **CK-MB** showed higher relevance

## Data Preprocessing
- Converted the target variable (Result) into numerical form using label encoding
- Split the dataset into training and testing sets (80% training, 20% testing)

## Machine Learning Models Used
The following classification models were trained and tested:
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier

## Model Performance
- Decision Tree achieved an accuracy of around **98%**
- Random Forest achieved an accuracy of around **97%**
- XGBoost achieved the best performance with an accuracy of approximately **98%**

Confusion matrices were used to analyze prediction performance in detail.

## Feature Importance
Feature importance analysis revealed that:
- **Troponin** is the most important feature for prediction
- **CK-MB** is the second most influential feature
- Age and blood sugar have moderate impact
- Blood pressure features contribute less compared to cardiac markers

## Model Saving
The trained XGBoost model was saved using `joblib` for future use or deployment.

## Tools & Libraries Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost

## Key Learnings
- Cardiac markers play a crucial role in heart attack prediction
- Ensemble models perform better than single decision trees
- Feature importance helps in understanding medical relevance of inputs
