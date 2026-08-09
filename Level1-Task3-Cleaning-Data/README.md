# Level 1 - Task 3: Cleaning Data

## 📌 Project Overview

This project is part of the **Oasis Infobyte Data Analytics Internship**.

The objective of this task is to clean and preprocess a messy **Titanic dataset** and transform it into a clean and analysis-ready dataset.

The project focuses on identifying missing values, detecting duplicate records, standardising inconsistent data formats, handling outliers, correcting data types, and comparing the dataset before and after cleaning.

---

## 🎯 Project Objective

The main objectives of this project are:

- Identify and handle missing values.
- Detect and remove duplicate records.
- Standardise inconsistent categorical values.
- Detect and analyse potential outliers.
- Handle outliers based on data context.
- Correct and verify data types.
- Compare the dataset before and after cleaning.
- Prepare a clean and analysis-ready dataset.
- Save the cleaned dataset for further analysis.

---

## 🛠️ Tools & Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📂 Dataset

The project uses the **Titanic Dataset**.

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

### Initial Dataset Shape

The original dataset contained:

- **891 rows**
- **12 columns**

---

## 🔍 Initial Data Inspection

The dataset was initially inspected using Pandas functions such as:

- `head()`
- `shape`
- `info()`
- `dtypes`
- `isnull().sum()`
- `duplicated().sum()`

The initial inspection helped identify missing values, data types, and duplicate records.

---

## 🧹 Data Cleaning Process

### 1. Missing Value Analysis

Missing values were identified in the dataset before performing the cleaning process.

The main columns requiring treatment were:

- `Age`
- `Cabin`
- `Embarked`

---

### 2. Handling Missing Age Values

The `Age` column contained missing values.

Instead of removing these records, the missing values were replaced using the **median age**.

The median value used for imputation was:

**28.0**

After imputation, no missing values remained in the `Age` column.

---

### 3. Handling Missing Embarked Values

The `Embarked` column contained missing values.

The missing values were replaced using the **mode** of the column.

The mode used for imputation was:

**S**

After this treatment, no missing values remained in the `Embarked` column.

---

### 4. Handling the Cabin Column

The `Cabin` column had a very high proportion of missing values.

The percentage of missing values was approximately:

**77.10%**

Because such a large proportion of the column was missing, the `Cabin` column was removed instead of attempting to impute most of its values.

This helped improve the overall quality and reliability of the cleaned dataset.

---

## 🔄 Duplicate Data Handling

Duplicate records were checked using Pandas.

The analysis found:

**0 duplicate rows**

Therefore, no rows were removed during duplicate removal.

The dataset remained at **891 rows** after this step.

---

## ✨ Data Standardisation

Categorical values were checked for consistency and standardised.

### Sex Column

The `Sex` column was standardised using consistent capitalization.

Before standardisation:

```text
male
female
