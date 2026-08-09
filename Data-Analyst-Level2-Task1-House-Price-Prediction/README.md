# House Price Prediction Using Linear Regression

## Project Overview

This project develops a machine learning model to predict house prices based on property characteristics such as area, bedrooms, bathrooms, stories, parking, location-related features, and other facilities.

The project follows an end-to-end machine learning workflow including exploratory data analysis, preprocessing, feature encoding, model training, evaluation, and interpretation.

## Objectives

- Explore the housing dataset.
- Analyze the distribution of house prices.
- Identify important predictors of house prices.
- Handle categorical variables using One-Hot Encoding.
- Analyze correlations between numerical variables.
- Train a Linear Regression model.
- Evaluate model performance using MSE, RMSE, and R².
- Analyze residuals and model coefficients.
- Compare Linear Regression with Ridge Regression.

## Dataset

The project uses the `Housing.csv` dataset containing housing property information and house prices.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Preprocessing

The dataset was checked for missing values and data types.

Categorical features were converted into numerical representations using One-Hot Encoding.

## Exploratory Data Analysis

The project includes:

- Descriptive statistics
- Missing value analysis
- House price distribution
- Correlation analysis
- Correlation heatmap

## Machine Learning

### Linear Regression

A Linear Regression model was trained using an 80/20 train-test split.

### Model Evaluation

The model was evaluated using:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

### Residual Analysis

A residual plot was created to examine the distribution of prediction errors.

### Coefficient Analysis

Model coefficients were analyzed to identify features with relatively strong positive or negative effects on predicted house prices.

## Ridge Regression

As a bonus, Ridge Regression was trained and compared with Linear Regression.

### Results

| Model | RMSE | R² Score |
|---|---:|---:|
| Linear Regression | 1,324,507 | 0.6529 |
| Ridge Regression | 1,325,320 | 0.6525 |

Linear Regression performed slightly better than Ridge Regression on the test dataset.

## Key Findings

- Area showed a strong positive relationship with house price.
- Bathrooms also showed a strong positive relationship with price.
- Several property facilities had positive model coefficients.
- The Linear Regression model achieved an R² score of approximately 0.653.

## Business Recommendations

1. Consider property size and facilities when estimating house prices.
2. Focus on amenities that contribute positively to property value.
3. Use data-driven regression models as a supporting tool for real-estate pricing decisions.

## Conclusion

This project demonstrates an end-to-end machine learning workflow for house price prediction, from exploratory data analysis and preprocessing to model evaluation and interpretation.
