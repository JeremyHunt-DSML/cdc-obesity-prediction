# 🩺 US Obesity Predictive Modeling & Analysis

[![View on nbviewer](https://img.shields.io/badge/Open_in-nbviewer-orange.svg)](https://nbviewer.org/github/JeremyHunt-DSML/cdc-obesity-prediction/blob/main/obesity_prediction_model.ipynb)

## Project Overview
This project performs a comprehensive Exploratory Data Analysis (EDA) and deploys machine learning models to understand the drivers of obesity in the United States. Utilizing the CDC's Behavioral Risk Factor Surveillance System (BRFSS) dataset, this analysis explores demographic, geographic, and temporal variables to predict obesity rates.

## The Approach
1. **Exploratory Data Analysis (EDA):** Investigated the BRFSS dataset to identify key features and trends related to obesity across different states and demographics.
2. **Feature Engineering:** Selected and prepared appropriate predictors, managing noise and ensuring statistical significance for modeling.
3. **Machine Learning Modeling:** Deployed and evaluated multiple algorithms to predict the outcome variable (`Data_Value` / Obesity Rate).

## Technologies & Libraries Used
* **Python 3**
* **Pandas & NumPy** (Data manipulation)
* **Scikit-Learn** (Machine Learning: Logistic Regression, Random Forest)
* **Matplotlib & Seaborn** (Data visualization and EDA)

## Key Insights & Model Evaluation
One of the core findings of this project is that "more complex" does not always mean "better" in machine learning. 
* **Model Performance:** A simpler, linear **Logistic Regression** model proved highly resilient and performed exceptionally well.
* **Handling Noise:** The Logistic Regression model successfully utilized predictive features from `YearStart` and demographics while effectively ignoring the noise introduced by the `Sample_Size` feature. 
* **Overfitting Avoidance:** Conversely, the more complex **Random Forest** algorithm was tripped up by that same noise, demonstrating the critical importance of feature selection and algorithm matching in predictive analytics.
