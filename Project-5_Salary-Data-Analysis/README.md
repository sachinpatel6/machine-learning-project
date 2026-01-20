## Salary Prediction using Machine Learning

## Project Overview
In this project, I worked on a salary dataset to understand how factors like age, education level, job title, and years of experience affect a person’s salary.
The main objective was to build machine learning models that can predict salary based on employee details.

## Dataset
The dataset contains 375 records, and after removing missing values, 373 records were used for modeling.
Columns in the dataset:
- Age
- Gender
- Education Level
- Job Title
- Years of Experience
- Salary (Target Variable)

The dataset is small but well-structured and suitable for regression-based prediction.


## Exploratory Data Analysis (EDA)
Used head(), info(), shape(), and describe() to understand the dataset
Visualized age distribution using histogram
Used a correlation heatmap to analyze relationships between variables

## Key Observations:
Years of Experience has a very strong correlation with Salary
Age is also highly correlated with Salary
Education Level has a moderate impact
Gender has almost no effect on Salary

This shows that salary growth is mostly driven by experience and age, not gender.

## Data Preprocessing
Removed missing values using dropna()
Converted categorical columns into numerical form using Label Encoding:
Gender
Education Level
Job Title

## Split the dataset into:
80% training data
20% testing data

## Machine Learning Models Used
The following regression models were trained and compared:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

## Model Performance
Models were evaluated using:
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
R² Score

## Performance Summary:
Linear Regression gave decent results but missed complex patterns
Decision Tree improved performance slightly
Random Forest Regressor performed the best
Gradient Boosting also performed well but slightly lower than Random Forest
Best Model: Random Forest Regressor
R² Score: **~ 0.94**
This indicates that ensemble models handle salary prediction better than simple models.

## Feature Importance
Feature importance analysis from the Random Forest model showed:
Most Important Features:
1. Age
2. Years of Experience
3. Job Title
4. Education Level
5. Gender
This confirms that experience and age are the strongest factors in salary prediction, while gender has very little impact.

## Tools & Libraries Used
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn

## Key Learnings
Salary is strongly influenced by experience and age
Gender does not significantly affect salary prediction
Ensemble models like Random Forest give higher accuracy
Feature importance helps in understanding real-world salary trends, not just predictions
