# California_housing_price_capstone3

A comprehensive machine learning project for predicting median house values in California using advanced regression techniques and feature engineering.

📋 Table of Contents
Project Overview

Business Problem

Dataset

Methodology

Installation

Usage

Results

Model Performance

Key Findings

Project Structure

Limitations

Future Improvements

🎯 Project Overview
This project implements a complete machine learning pipeline to predict median house prices in California districts based on the 1990 census data. The solution addresses challenges, including feature engineering, handling missing values, and model optimization to provide accurate housing price predictions.

Key Features:

Comprehensive EDA with geographical visualizations

Advanced feature engineering to reduce multicollinearity

Multiple regression models comparison (6 algorithms)

Hyperparameter tuning with GridSearchCV

Complete model evaluation with residual analysis

Production-ready model serialization

📊 Business Problem Understanding
Context
The dataset contains housing census data from California in 1990. This is a popular geographical regression dataset used to test machine learning algorithms. Each row represents one block group in California. The main objective is to predict median house value (median_house_value) in each block based on geographical and demographic features.

Problem Statement
Property valuation is a complex problem influenced by multiple factors like location, house age, room count, and resident income. For investors, property developers, or local governments, having accurate house price prediction tools is crucial for:

Investment decisions: Identifying areas where property values are likely to increase

Fair property valuation: Ensuring sale/purchase prices align with market values

Urban planning: Understanding relationships between demographic/geographical factors and property values

Market trend analysis: Estimating potential property value increases/decreases

Project Goals
Develop a regression model to predict median_house_value

Identify the most influential features (location, income, ocean proximity)

Provide business insights for stakeholders regarding property planning and investment

📁 Dataset
The project uses the California Housing Dataset, containing information from the 1990 California census.

Features:
longitude: Geographical position (westward decreasing)

latitude: Geographical position (northward increasing)

housing_median_age: Median age of houses in the block

total_rooms: Total number of rooms in block

total_bedrooms: Total number of bedrooms in block

population: Total population in block

households: Total number of households

median_income: Median household income (tens of thousands of USD)

ocean_proximity: Proximity to ocean (categorical)

Target:
median_house_value: Median house value for California districts (USD)

🛠️ Methodology
1. Data Preprocessing
Missing value handling for total_bedrooms

Duplicate detection and removal

Outlier analysis using IQR method

Exploratory Data Analysis (EDA) with geographical mapping

2. Feature Engineering
Created new features:

rooms_per_household: Total rooms ÷ households

bedrooms_per_room: Total bedrooms ÷ total rooms

population_per_household: Population ÷ households

Dropped original correlated features to reduce multicollinearity

Label encoding for categorical features

3. Modeling Approaches
Tested 6 regression algorithms:

Linear Regression

K-Neighbors Regressor

Decision Tree Regressor

Random Forest Regressor

Support Vector Regressor (SVR)

LightGBM Regressor

4. Model Evaluation
Primary metrics:

RMSE (Root Mean Squared Error): Measures average error magnitude

MAE (Mean Absolute Error): Average absolute difference

MAPE (Mean Absolute Percentage Error): Percentage error

R² Score: Variance explained by the model
