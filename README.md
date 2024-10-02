# Academic Projects
This repository features a selection of projects from my Master’s program:

## Python and Analytics Systems Technology

Date: 12/17/2023
Focus: Analyzed credit card payment behaviors in Taiwan to assess default prediction methods using diverse datasets.
Data Management & Big Data

## Project Report
## Electric Vehicle Population Dataset
Date: 06/30/2023
Team: Anoushka Hazari, Xuanyu Bao
Focus: Used big data to analyze factors influencing EV adoption and market trends to support sustainable transportation.

## Enterprise Risk Management Assessment Report

Date: 03/30/2024
Focus: Assessed risks for OtakuGear Emporium, an anime merchandise startup, with a comprehensive risk response plan.

## Communication and Visualization for Data Analytics

Date: 03/31/2023
Focus: Analyzed 2015 census data on tree species in New York City to highlight urban tree distribution and benefits.
Capstone Project

## Project: Sneaker Resale Market Analysis for Arbit Company

### Introduction
In this project, we aim to predict the sold prices of sneakers using various features, applying machine learning techniques to uncover meaningful insights and correlations within the dataset.

### Data Preprocessing

#### Label Encoding
To analyze the relationship between different variables and prepare our dataset for predictive modeling, we utilized the `LabelEncoder` from the `scikit-learn` library. This process involved transforming categorical variables into numerical representations. The rationale behind this transformation was to enable the computation of correlation coefficients, helping us understand the relationships between various features in our dataset.

Each categorical variable, such as the condition, gender, source, brand, color, silhouette, and collaboration status of sneakers, was encoded into numerical values using the `LabelEncoder`. This encoding ensured that the data was in a format suitable for correlation analysis and subsequent predictive modeling tasks.

The primary goal of this preprocessing step was to construct a correlation matrix, providing a visual representation of the pairwise correlations between different variables. By examining this matrix, we could identify which features were most strongly correlated with each other and with the target variable, the sold price of sneakers.

Overall, applying `LabelEncoder` was essential for ensuring that our dataset was appropriately formatted and ready for analysis. It allowed us to uncover meaningful insights into the relationships between variables, guiding our decisions in selecting the most relevant features for predictive modeling in the subsequent stages of our project.

### Correlation Matrix
Upon examining the correlation matrix, notable observations emerged regarding the relationships between various variables. Particularly, the sold price variable demonstrated the strongest correlation with retail price. Additionally, a high correlation was noted between `is_collab` and `Collaborator`, as well as between `is_collab` and `silhouette`, indicating potential associations between collaboration status and sneaker characteristics. Furthermore, `is_collab` exhibited significant correlations with brand, suggesting possible dependencies between collaboration status and brand affiliations.

Numerous other correlations were identified, but given the focus on sold price as the target variable for predictive modeling, the most pertinent associations were noted. Notably, retail price displayed the highest correlation with sold price, followed by `is_collab` and `Collaborator`. This insight underscores the significance of these variables in influencing the sold price of sneakers. As such, these findings inform the selection of features for predictive modeling, prioritizing those with the strongest correlations with the target variable.

### Predictive Modeling and Its Evaluation
Upon evaluating the performance of various regression models, it became evident that traditional linear regression techniques, including Linear, Lasso, and Ridge regression, yielded unsatisfactory results in terms of predictive accuracy. Despite their application, the R-squared values remained notably low, indicating that these models could not sufficiently explain the variance in the target variable, sold price. Consequently, alternative approaches were explored to enhance predictive capabilities.

Subsequently, Random Forest Regression, a more sophisticated ensemble learning method, was employed. This decision was motivated by the desire to improve predictive performance beyond the limitations of linear regression models. Remarkably, Random Forest Regression demonstrated significantly superior performance, as evidenced by a substantially lower Mean Squared Error (MSE) and a substantially higher R-squared value (MSE: 22426.16, R-squared: 0.75). These metrics indicated a much better fit of the model to the data, suggesting that Random Forest Regression could more accurately predict the sold price of sneakers based on the input features.

The output from the Random Forest Regression model provides two key metrics: Mean Squared Error (MSE) and R-squared (R²).

1. **Mean Squared Error (MSE)**: This metric measures the average squared difference between the actual and predicted values of the target variable (sold price). In this context, the MSE value of 22426.16 indicates that, on average, the squared difference between the actual and predicted sold prices is approximately 22426.16. A lower MSE suggests that the model's predictions are closer to the actual values, indicating better overall performance.
   
2. **R-squared (R²)**: This metric represents the proportion of variance in the target variable (sold price) that is explained by the independent variables (features) in the model. The R-squared value of 0.75 indicates that approximately 75% of the variance in sold prices can be explained by the features included in the Random Forest Regression model. A higher R-squared value suggests that the model fits the data well and provides reliable predictions.

In summary, the output suggests that the Random Forest Regression model is performing well, with relatively low MSE and a high R-squared value, indicating that it can effectively predict the sold prices of sneakers based on the selected features.

Furthermore, a feature importance analysis was conducted to identify the most influential predictors in the Random Forest Regression model. Notably, the analysis revealed that retail price emerged as the most critical feature, contributing approximately 48.47% to the predictive power of the model. Other important features included silhouette, color, and collaboration status, which collectively played significant roles in determining the sold price of sneakers. These insights provided valuable guidance for feature selection and model refinement in subsequent iterations of the predictive modeling process.

### Conclusion
This project highlights the importance of preprocessing steps, such as label encoding, in preparing data for predictive modeling. By utilizing Random Forest Regression, we achieved a substantial improvement in predictive accuracy, allowing for meaningful insights into sneaker pricing.


