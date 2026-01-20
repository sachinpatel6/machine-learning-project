# Insurance Cost Prediction using Machine Learning

## Project Overview
In this project, I worked on a medical insurance dataset to understand what factors
affect insurance charges and to build a model that can predict the cost based on
customer details like age, BMI, smoking habits, and region.

## Dataset
The dataset contains **1338 records** with the following columns:
- age  
- sex  
- bmi  
- children  
- smoker  
- region  
- charges (target variable)

The dataset is clean and does not contain any missing values.

## Exploratory Data Analysis (EDA)
- Looked at basic statistics and data distribution
- Used correlation heatmaps to understand relationships between features
- Found that smoking status has a strong impact on insurance charges

## Data Preprocessing
- Converted categorical columns (sex, smoker, region) into numerical form using label encoding
- Scaled numerical features using StandardScaler
- Split the data into training and testing sets in an 80:20 ratio

## Machine Learning Models Used
The following models were trained and compared:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

## Model Performance
The models were evaluated using:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R² Score

Among all the models, **Gradient Boosting Regressor performed the best**, achieving an
R² score of approximately **0.87**.

## Feature Importance
From feature importance analysis:
- Smoking status turned out to be the most important factor
- BMI and age also play a significant role in determining insurance cost
- Number of children and region have relatively less impact

## Tools & Libraries Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## Key Learnings
- Lifestyle factors like smoking greatly influence medical insurance costs
- Ensemble models give better results than simple linear models
- Feature importance helps in understanding the problem from a business perspective
