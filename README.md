# Academic Projects
This repository features a selection of projects from my Master’s program:

## 1)Credit Card Default Prediction Analysis(ALY6140)

### Business Questions
- **Credit Risk:** What factors influence defaults?
- **Segmentation:** How do spending patterns vary by demographics?
### Dataset Overview
- **Size:** 30,000 instances
- **Key Variables:** LIMIT_BAL, AGE, SEX, EDUCATION, MARRIAGE
### Data Cleaning
- Cleaned 10% of data with missing or erroneous values.
### EDA Insights
- **Correlation:** Strong relationships in payment and billing amounts.
### Modeling
- **Logistic Regression:** 78% accuracy.
- **Decision Tree:** 72% accuracy.
- **Random Forest:** 82% accuracy (best performer).

### Conclusion
- Random Forest model provides the best prediction for defaults.

## 2)Project: Sneaker Resale Market Analysis for Arbit Company(BiweeklycapstoneF.ipynb)

### Introduction
This project aims to predict the sold prices of sneakers using various features and machine learning techniques.

### Data Preprocessing

#### Label Encoding
We used `LabelEncoder` from the `scikit-learn` library to transform categorical variables (e.g., condition, gender, brand) into numerical values. This step enabled the computation of correlation coefficients, helping us understand relationships between features and the target variable, sold price. The encoding facilitated the creation of a correlation matrix to identify significant feature associations.

### Correlation Matrix
The correlation matrix revealed that sold price had the strongest correlation with retail price. High correlations were also observed between `is_collab` and `Collaborator`, and with brand. These insights guided our feature selection for predictive modeling.

### Predictive Modeling and Evaluation
Initial attempts with linear regression models (Linear, Lasso, Ridge) yielded low R-squared values, indicating poor performance. We then employed Random Forest Regression, which significantly improved our results (MSE: 22426.16, R-squared: 0.75). This model effectively predicts sold prices, with retail price being the most influential feature, contributing approximately 48.47% to its predictive power.

### Conclusion
This project underscores the importance of data preprocessing and the efficacy of Random Forest Regression in accurately predicting sneaker prices. Insights gained will guide future feature selection and model enhancements.


## 3)Project Report
## Electric Vehicle Population Dataset(Eco Drive)
Date: 06/30/2023
Team: Anoushka Hazari, Xuanyu Bao
Focus: Used big data to analyze factors influencing EV adoption and market trends to support sustainable transportation.

## 4)Enterprise Risk Management Assessment Report

Date: 03/30/2024
Focus: Assessed risks for OtakuGear Emporium, an anime merchandise startup, with a comprehensive risk response plan.

## 5)Communication and Visualization for Data Analytics(Census2 , Census3)

Date: 03/31/2023
Focus: Analyzed 2015 census data on tree species in New York City to highlight urban tree distribution and benefits.
Capstone Project

