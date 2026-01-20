# Wine Quality Analysis using Machine Learning

## Project Overview
This project focuses on analyzing wine quality data and predicting wine type
based on different chemical properties.
The main goal is to understand which factors influence wine quality and
evaluate machine learning models for classification.

## Dataset
The dataset contains **6497 wine samples** with the following features:
- Fixed acidity  
- Volatile acidity  
- Citric acid  
- Residual sugar  
- Chlorides  
- Free sulfur dioxide  
- Total sulfur dioxide  
- Density  
- pH  
- Sulphates  
- Alcohol  
- Quality  
- Type (target variable)

The dataset is clean and does not contain any missing values.

## Exploratory Data Analysis (EDA)
- Checked dataset structure, size, and summary statistics
- Analyzed distributions of chemical properties
- Used correlation heatmaps to understand relationships between features
- Observed strong relationships between alcohol, sulphates, and wine quality

## Data Preprocessing
- Converted wine type into numerical format using Label Encoding
- Split the data into training and testing sets (80% training, 20% testing)

## Machine Learning Models Used
The following classification models were trained and evaluated:
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier

## Model Performance
- Decision Tree achieved an accuracy of around **98%**
- Random Forest achieved the best performance with an accuracy of around **99.5%**
- XGBoost also performed very well with an accuracy close to **99%**

Confusion matrices were used to analyze correct and incorrect predictions.

## Feature Importance
Feature importance analysis showed that:
- **Chlorides** and **Total Sulfur Dioxide** are the most influential features
- Volatile acidity and fixed acidity have moderate impact
- Density has relatively lower importance

## Model Saving
The trained model was saved using `joblib` for future use or deployment.

## Tools & Libraries Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost

## Key Learnings
- Chemical properties strongly affect wine quality and type
- Ensemble models like Random Forest and XGBoost perform better than simple models
- Feature importance helps in understanding real-world impact of variables
