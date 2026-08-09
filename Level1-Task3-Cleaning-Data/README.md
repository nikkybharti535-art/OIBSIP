# Data Cleaning Project

## Project Overview

This project demonstrates professional data cleaning techniques using a deliberately messy dataset. The objective is to transform raw data into a clean and analysis-ready dataset while documenting the decisions made during the cleaning process.

## Objectives

- Inspect the quality of the dataset.
- Identify missing values.
- Detect and remove duplicate records.
- Standardize inconsistent data.
- Detect numerical outliers.
- Correct inappropriate data types.
- Compare the dataset before and after cleaning.
- Export the cleaned dataset.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Quality Analysis

The dataset was initially inspected for:

- Missing values
- Duplicate rows
- Incorrect data types
- Range anomalies
- Numerical outliers

## Data Cleaning Process

### Missing Values

Missing values were analyzed column by column and handled using appropriate strategies based on the characteristics of each variable.

### Duplicate Removal

Duplicate rows were identified and removed to prevent repeated observations from affecting the analysis.

### Standardization

Inconsistent formats and categorical values were standardized to maintain consistency throughout the dataset.

### Outlier Detection

The IQR method was used to identify potential outliers in numerical variables. The detected observations were reviewed before deciding whether they should be retained or handled.

### Data Type Correction

Columns were converted to appropriate data types to ensure that the cleaned dataset could be used reliably for further analysis.

## Before vs After

A comparison was created to evaluate:

- Null values
- Duplicate rows
- Number of records
- Data types

before and after the cleaning process.

## Output

The cleaned dataset was saved as a new CSV file for future analysis.

## Conclusion

The project demonstrates a systematic approach to data cleaning and highlights the importance of data quality before performing analysis or building machine learning models.
