# Level 1 - Task 3: Cleaning Data

## Project Overview

This project is part of the Oasis Infobyte Data Analytics Internship.

The objective of this task is to clean and preprocess the Titanic dataset and transform the raw dataset into a clean and analysis-ready dataset.

The project focuses on identifying missing values, checking duplicate records, handling missing data, standardising categorical values, detecting potential outliers, verifying data types, and validating the dataset after cleaning.

## Objectives

- Understand the structure of the Titanic dataset.
- Identify missing values.
- Check for duplicate records.
- Handle missing values appropriately.
- Remove columns with a high percentage of missing values.
- Standardise categorical values.
- Detect potential outliers.
- Analyse detected outliers using the IQR method.
- Verify data types.
- Validate the cleaned dataset.
- Prepare the dataset for further analysis.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset

The project uses the Titanic dataset.

The original dataset contains information about Titanic passengers, including:

- PassengerId
- Survived
- Pclass
- Name
- Sex
- Age
- SibSp
- Parch
- Ticket
- Fare
- Cabin
- Embarked

### Initial Dataset

The original dataset contained:

- 891 rows
- 12 columns

## Data Cleaning Process

### 1. Initial Data Inspection

The dataset was loaded using Pandas and inspected using:

- `head()`
- `shape`
- `info()`
- `dtypes`
- `isnull().sum()`
- `duplicated().sum()`

This helped identify the structure, data types, missing values, and duplicate records.

### 2. Missing Value Analysis

Missing values were checked across all columns.

The main columns requiring treatment were:

- Age
- Cabin
- Embarked

### 3. Handling Missing Values in Age

The Age column contained missing values.

The missing values were replaced using the median of the Age column.

Median Age:

28.0

Using the median helps preserve the records while reducing the influence of extreme values.

### 4. Handling Missing Values in Embarked

The Embarked column contained missing values.

The missing values were replaced using the mode of the column.

Mode:

S

### 5. Handling the Cabin Column

The Cabin column contained a very high percentage of missing values.

Approximately 77.10% of the values were missing.

Because such a large proportion of the column was missing, the Cabin column was removed instead of trying to impute most of its values.

### 6. Duplicate Records

Duplicate records were checked using Pandas.

Result:

0 duplicate rows

Therefore, no records were removed because of duplication.

### 7. Data Standardisation

Categorical values were checked and standardised for consistency.

The Sex column was standardised to:

- Male
- Female

The Embarked column was standardised to:

- S
- C
- Q

### 8. Outlier Detection

Potential outliers were identified using the Interquartile Range (IQR) method.

The IQR is calculated as:

IQR = Q3 - Q1

The lower and upper bounds were calculated as:

Lower Bound = Q1 - 1.5 × IQR

Upper Bound = Q3 + 1.5 × IQR

Outlier analysis was performed on:

- Age
- Fare
- SibSp
- Parch

### 9. Outlier Analysis Results

The potential outliers identified were:

- Age: 66
- Fare: 116
- SibSp: 46
- Parch: 213

Boxplots were used to visually inspect the numerical variables and their potential outliers.

### 10. Outlier Treatment

The detected outliers were not removed.

The reason for retaining them is that these values may represent valid real-world observations rather than incorrect data.

For example, higher Fare values may represent expensive tickets, while higher SibSp or Parch values may represent passengers travelling with larger families.

Therefore, the outliers were retained.

### 11. Data Type Verification

The data types of the columns were checked and verified during the cleaning process.

Numerical variables were maintained as numerical data types, while categorical variables were maintained as appropriate text/object data types.

## Visualisation

Visualisations were used to support the data-cleaning process.

Boxplots were created to inspect numerical variables and identify potential outliers.

The visualisations helped understand:

- Data distribution
- Spread of numerical values
- Potential extreme observations
- Possible outliers

## Key Findings

1. The original Titanic dataset contained 891 rows and 12 columns.

2. The dataset contained 0 duplicate records.

3. Missing values in the Age column were handled using median imputation.

4. The median value used for Age was 28.0.

5. Missing values in the Embarked column were handled using the mode value S.

6. The Cabin column contained approximately 77.10% missing values and was therefore removed.

7. Potential outliers were identified in Age, Fare, SibSp, and Parch using the IQR method.

8. The detected outliers were retained because they could represent valid observations.

9. Categorical values were standardised to maintain consistency.

10. After cleaning, the dataset contained 891 rows and 11 columns.

## Final Dataset

After completing the cleaning process:

- Original rows: 891
- Original columns: 12
- Duplicate rows removed: 0
- Cabin column: Removed
- Final rows: 891
- Final columns: 11

The final dataset is cleaner and more suitable for further analysis.

## Project Structure

Level1-Task3-Cleaning-Data/
│
├── README.md
├── Cleaning_Data.ipynb
├── Titanic-Dataset.csv
└── Cleaned_Titanic_Dataset.csv

## How to Run

1. Install the required Python libraries.

2. Open Jupyter Notebook.

3. Open `Cleaning_Data.ipynb`.

4. Keep the Titanic dataset in the same project folder.

5. Run the notebook cells sequentially to reproduce the complete data-cleaning process.

## Conclusion

This project demonstrates a complete data-cleaning and preprocessing workflow using the Titanic dataset.

The process included missing-value analysis, missing-value treatment, duplicate checking, categorical data standardisation, outlier detection using the IQR method, outlier evaluation, data-type verification, and final dataset validation.

The cleaning process improved the consistency and quality of the dataset while preserving potentially meaningful observations.

The final dataset can be used for further exploratory data analysis, visualisation, and machine learning applications.

## Author

Nikky Bharti

