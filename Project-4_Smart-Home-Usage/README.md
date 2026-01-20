# Smart Home Device Usage Analysis using Machine Learning

## Project Overview
This project analyzes smart home device usage data to understand user behavior,
energy consumption patterns, and factors affecting overall smart home efficiency.
Multiple machine learning models are used to predict smart home efficiency
and compare their performance.

## Dataset
The dataset contains **5403 records** with the following features:
- UserID  
- DeviceType  
- UsageHoursPerDay  
- EnergyConsumption  
- UserPreferences  
- MalfunctionIncidents  
- DeviceAgeMonths  
- SmartHomeEfficiency (target variable)

The dataset is clean with **no missing or duplicate values**.

## Exploratory Data Analysis (EDA)
- Checked dataset shape, structure, and summary statistics
- Analyzed skewness of numerical features
- Visualized usage patterns using histograms
- Used correlation heatmaps to understand relationships between features

### Key Observations
- User preferences show a strong positive correlation with smart home efficiency
- Higher energy consumption negatively affects efficiency
- Device age and malfunction incidents also impact efficiency

## Data Preprocessing
- Removed duplicate records (none found)
- Encoded categorical feature `DeviceType` using Label Encoding
- Split data into training and testing sets (80% training, 20% testing)

## Machine Learning Models Used
The following classification models were trained and evaluated:
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier
- Logistic Regression
- Support Vector Machine (SVM)

## Model Performance
Model accuracy comparison:
- Decision Tree: **~95.28%**
- Random Forest: **~95.19%**
- XGBoost: **~95.10%**
- SVM: **~90.29%**
- Logistic Regression: **~87.42%**

Tree-based models performed better compared to linear models.

Confusion matrices were used to analyze prediction performance for each model.

## Feature Importance
Feature importance analysis (Random Forest) showed that:
- **UserPreferences** is the most important feature
- UsageHoursPerDay and EnergyConsumption have significant impact
- DeviceAgeMonths and UserID have moderate influence

## Tools & Libraries Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost

## Key Learnings
- User behavior plays a major role in smart home efficiency
- Ensemble models provide better accuracy and stability
- Feature importance helps identify actionable insights for energy optimization
