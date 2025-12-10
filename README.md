**California Housing Price Prediction: Capstone Project 3**
This project aims to build a machine learning model that can predict median house prices in California based on 1990 census data. The model is developed using an end-to-end approach: from data exploration, feature engineering, model training, to evaluation and model storage for production.

Key Features:

- Comprehensive EDA with geographical visualizations
- Feature engineering to reduce multicollinearity
- Testing of 6 different regression algorithms
- Hyperparameter tuning with GridSearchCV
- Comprehensive evaluation with residual analysis

Model saved in .pkl format for deployment

🎯 Business Problem
**Background**
1990 California housing census data is used to test the model's ability to predict median_house_value. Each row represents one block group. Accurate house price prediction is crucial for:
- Real Estate Agents
- Government
Project Goals
- Build a regression model to predict median_house_value
- Identify the most influential features on house prices
- Provide data-driven business insights for decision making

📊 Dataset
**Data Source**
Name: California Housing Dataset (1990)
Number of rows: 14,448
Number of features: 10 (9 features + 1 target)

**Variables**
Column	Type	Description
**longitude** float	Longitude position (decreases westward)
**latitude**	float	Latitude position (increases northward)
**housing_median_age**	float	Median age of houses in the block
**total_rooms**	float	Total rooms in block
**total_bedrooms**	float	Total bedrooms (has missing values)
**population**	float	Population in block
**households**	float	Number of households
**median_income**	float	Median income (in tens of thousands USD)
**ocean_proximity**	object	Proximity to ocean category
**median_house_value**	float	Target: Median house value (USD)

🔧 Methodology
1. Data Preprocessing
Handle missing values in total_bedrooms with mean imputation
Detect and remove duplicates
Outlier analysis using IQR
Encoding ocean_proximity with Label Encoding
2. Feature Engineering
Drop original features to avoid multicollinearity
3. Modeling
6 algorithms tested:
- Linear Regression
- K-Neighbors Regressor
- Decision Tree Regressor
- Random Forest Regressor
- Support Vector Regressor (SVR)
- LightGBM Regressor

4. Model Evaluation
**RMSE (Root Mean Squared Error)**
**MAE (Mean Absolute Error)**
**MAPE (Mean Absolute Percentage Error)**
**R² Score**

5. Hyperparameter Tuning
GridSearchCV on LightGBM with 5-fold cross-validation.

