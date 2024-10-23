# Used Car Price Prediction 🚗💰

This project implements a **Machine Learning** model to predict the prices of used cars based on various features such as mileage, fuel type, and engine specifications. The dataset is an aggregation of popular Kaggle datasets, focusing on the Indian car market.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Usage](#usage)
- [Conclusion](#conclusion)

## Project Overview
The goal of this project is to predict the price of used cars using machine learning techniques. We explore multiple models, including Linear Regression, Random Forest, and XGBoost, to find the best-performing one for this regression problem.

## Dataset
- Aggregated from [**top 4 Kaggle datasets**](https://www.kaggle.com/datasets/satvshr/top-4-used-car-sales-datasets-combined) on used car prices in India.
- Contains information on **32,200 cars** with features like `brand`, `model`, `mileage`, `engine`, `seats`, and more.
- The target variable is the `price` of the car.

## Features
Here are some of the key features used for the prediction:
- **Brand & Model**: Car brand and model type.
- **Fuel Type & Transmission**: Fuel type (petrol/diesel) and transmission (manual/automatic).
- **Mileage & Engine**: Mileage (kmpl) and engine displacement (cc).

## Data Preprocessing
- Handled missing data by imputing or dropping columns with high missing values.
- Converted categorical variables into numeric using **One-Hot Encoding**.
- **MinMaxScaler** used for scaling numerical features.
  
## Exploratory Data Analysis (EDA)
We performed a comprehensive EDA to understand the relationships between various features and the car price:
- **Univariate Analysis**: Distribution of numerical features like mileage, price, etc.
- **Bivariate Analysis**: Examined the relationship between price and other features using **box plots**, **scatter plots**, and **heatmaps** for correlations.

## Feature Engineering
- Created new features.
- Applied **PCA** to select the most important features for the model.
  
## Modeling
We trained several models, including:
- **Linear Regression**
- **Random Forest Regressor**
- **Gradient Boosting**
- **Support Vector Regressor (SVR)**

The **Random Forest** and **XGBoost** models performed the best, achieving high accuracy with an R² of 99.2%.

## Evaluation
We used the following metrics for model evaluation:
- **Mean Squared Error (MSE)**
- **R² Score**

## Conclusion
- The **Random Forest** and **XGBoost** models provided the best results for this dataset.
- This project demonstrates how **machine learning** can be applied to predict used car prices effectively.
