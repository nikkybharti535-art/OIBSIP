# Data Analyst - Level 2 - Task 1: House Price Prediction

## 📌 Project Overview

This project is part of the Oasis Infobyte Data Analytics Internship.

The objective of this task is to build a machine learning model that predicts house prices based on the available housing features.

The project covers data loading, data inspection, preprocessing, exploratory data analysis, feature selection, model training, prediction, model evaluation, and visualisation.

---

## 🎯 Objectives

The main objectives of this project are:

- Understand the structure of the housing dataset.
- Inspect the dataset for missing values and duplicate records.
- Perform data cleaning and preprocessing.
- Explore the relationship between different features and house prices.
- Select relevant features for prediction.
- Split the data into training and testing sets.
- Train a machine learning regression model.
- Predict house prices for unseen data.
- Evaluate the performance of the prediction model.
- Visualise actual and predicted house prices.

---

## 🛠️ Tools & Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📂 Dataset

The project uses a house price dataset containing information about residential properties and their corresponding prices.

The dataset was inspected to understand:

- Number of rows and columns
- Column names
- Data types
- Missing values
- Duplicate records
- Numerical features
- Target variable
- Relationships between variables

---

## 🔍 Data Inspection

The dataset was initially inspected using Pandas functions such as:

- `head()`
- `shape`
- `info()`
- `describe()`
- `isnull().sum()`
- `duplicated().sum()`

These checks helped understand the structure and quality of the dataset before building the prediction model.

---

## 🧹 Data Preprocessing

The dataset was prepared before applying machine learning.

The preprocessing workflow included:

- Checking missing values.
- Checking duplicate records.
- Inspecting data types.
- Selecting relevant features.
- Preparing the input variables.
- Preparing the target variable.
- Converting the data into a suitable format for machine learning.

---

## 📊 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the dataset and identify patterns related to house prices.

The analysis included:

- Descriptive statistics
- Feature distributions
- Correlation analysis
- Relationship between numerical features and house prices
- Visualisation of important variables

Matplotlib and Seaborn were used to create graphs and plots for better interpretation.

---

## 🎯 Feature Selection

The available housing features were analysed to determine their usefulness for predicting house prices.

The selected features were used as input variables, while the house price was used as the target variable.

The basic prediction structure was:

**Input Features → Machine Learning Model → Predicted House Price**

---

## ✂️ Train-Test Split

The dataset was divided into training and testing datasets.

The training dataset was used to train the machine learning model, while the testing dataset was used to evaluate the model on previously unseen data.

This helps measure how well the model can generalise to new observations.

---

## 🤖 Machine Learning Model

A regression-based machine learning approach was used for house price prediction.

The model was trained using the selected housing features and the corresponding house prices.

After training, the model was used to generate predicted house prices for the test dataset.

---

## 📈 Model Prediction

The trained model generated predicted prices for the test observations.

The predicted values were compared with the actual house prices to understand the performance of the model.

The comparison helps identify how closely the model's predictions match the actual values.

---

## 📊 Model Evaluation

The prediction model was evaluated using appropriate regression evaluation metrics.

Model evaluation helps determine the accuracy and effectiveness of the house price prediction model.

The evaluation included comparison between:

- Actual House Prices
- Predicted House Prices

The detailed evaluation results are available in the Jupyter Notebook.

---

## 📉 Visualisation

Visualisations were created to understand the data and model performance.

The analysis includes:

- Feature distributions
- Correlation analysis
- Relationships between housing features and price
- Actual vs Predicted house prices

These visualisations make it easier to understand patterns in the data and evaluate prediction performance.

---

## 💡 Key Insights

The project demonstrates:

- How real-world housing data can be prepared for machine learning.
- How exploratory data analysis helps understand important housing features.
- How relevant features can be used to predict house prices.
- How regression models can be applied to prediction problems.
- How training and testing data are used to evaluate a model.
- How actual and predicted values can be compared visually.
- How evaluation metrics help measure model performance.

---

## 📁 Project Structure

```text
Data-Analyst-Level2-Task1-House-Price-Prediction/
│
├── README.md
├── House_Price_Prediction.ipynb
└── dataset.csv
