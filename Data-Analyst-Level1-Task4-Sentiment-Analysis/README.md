# Level 1 - Task 4: Sentiment Analysis

## 📌 Project Overview

This project is part of the Oasis Infobyte Data Analytics Internship.

The objective of this task is to perform Sentiment Analysis on text data and classify user reviews into different sentiment categories.

The project includes text preprocessing, feature extraction, machine learning-based sentiment classification, model evaluation, visualisation, and VADER-based sentiment analysis.

The analysis helps understand whether user reviews express positive, negative, or neutral opinions.

---

## 🎯 Objectives

The main objectives of this project are:

- Load and inspect the sentiment analysis dataset.
- Clean and preprocess the review text.
- Convert text data into numerical features.
- Split the dataset into training and testing sets.
- Build machine learning models for sentiment classification.
- Compare model performance.
- Evaluate the classification results.
- Visualise sentiment distribution.
- Perform sentiment analysis using VADER.
- Analyse sentiment across different app categories.
- Extract meaningful insights from user reviews.

---

## 🛠️ Tools & Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- WordCloud
- VADER Sentiment
- Jupyter Notebook

---

## 📂 Dataset

The project uses user review data for sentiment analysis.

The dataset contains text reviews along with sentiment-related information.

Important fields used during the analysis include:

- App
- Translated_Review
- Sentiment
- Sentiment_Polarity
- Sentiment_Subjectivity

Additional VADER-based fields were created during the analysis:

- compound_score
- VADER_Sentiment

---

## 🔍 Data Inspection and Preprocessing

The dataset was first loaded and inspected to understand its structure.

The following checks were performed:

- Dataset shape
- Column names
- Data types
- Missing values
- Duplicate records
- Review text availability

Rows without valid review text were handled before performing sentiment analysis.

The review text was then prepared for further text-based analysis.

---

## 🧹 Data Cleaning

The following preprocessing steps were performed:

- Checked for missing review text.
- Removed records where review text was unavailable for sentiment analysis.
- Checked duplicate records.
- Prepared the review text for feature extraction.
- Used the cleaned review data for sentiment classification.

This preprocessing helped improve the quality of the input data used by the models.

---

## 🔤 Text Feature Extraction

Since machine learning models cannot directly process raw text, the review text was converted into numerical features.

**TF-IDF (Term Frequency-Inverse Document Frequency)** was used for feature extraction.

TF-IDF represents the importance of words in a document relative to the complete collection of documents.

This transformed the review text into a numerical representation that could be used by machine learning algorithms.

---

## ✂️ Train-Test Split

The processed dataset was divided into training and testing data.

The dataset was split using an **80:20 ratio**:

- 80% Training Data
- 20% Testing Data

The training data was used to build the classification models, while the testing data was used to evaluate their performance on unseen reviews.

---

## 🤖 Machine Learning Models

Two machine learning classification models were used for sentiment classification.

### 1. Naive Bayes

A Naive Bayes classifier was trained using the TF-IDF features.

It was used to classify reviews into their corresponding sentiment categories.

### 2. Logistic Regression

Logistic Regression was also trained using the TF-IDF feature representation.

The model was evaluated on the testing dataset and its performance was compared with the Naive Bayes classifier.

---

## 📊 Model Evaluation

The trained models were evaluated using classification performance metrics.

The evaluation included:

- Accuracy
- Classification results
- Confusion Matrix

The confusion matrix was used to understand the number of correctly and incorrectly classified reviews for each sentiment class.

---

## 📈 Model Comparison

The performance of the Naive Bayes and Logistic Regression models was compared to determine how effectively each model classified the review sentiments.

The comparison helps identify which model performed better on the given dataset.

Detailed model outputs and evaluation results are available in the Jupyter Notebook.

---

## 📊 Sentiment Visualisation

Different visualisations were created to understand the sentiment distribution in the dataset.

The analysis included visual representations of:

- Positive reviews
- Negative reviews
- Neutral reviews
- Sentiment distribution

These visualisations make it easier to understand the overall opinion expressed by users.

---

## ☁️ WordCloud Analysis

A WordCloud was used to visualise frequently occurring words in the review dataset.

The WordCloud provides a quick overview of commonly used terms in user reviews.

Frequently appearing words can help identify common topics and themes discussed by users.

---

## 🧠 VADER Sentiment Analysis

VADER (Valence Aware Dictionary and sEntiment Reasoner) was also used for sentiment analysis.

VADER is a rule-based sentiment analysis tool that provides a compound sentiment score for text.

A new column was created:

`compound_score`

The compound score was then used to classify reviews into:

- Positive
- Neutral
- Negative

A new sentiment column was created:

`VADER_Sentiment`

Example output structure:

- Review text
- Compound score
- VADER sentiment

---

## 📊 Sentiment by App Category

The VADER sentiment results were further analysed according to app categories.

The analysis compared the number of:

- Negative reviews
- Neutral reviews
- Positive reviews

across different app categories.

This helps identify which categories receive comparatively more positive or negative user feedback.

---

## 🔍 Key Analysis Areas

The project covers the following major areas:

### Review Sentiment

User reviews were classified according to their expressed sentiment.

### Machine Learning Classification

Naive Bayes and Logistic Regression were used to classify review sentiments.

### Model Evaluation

The classification models were evaluated using accuracy and confusion matrices.

### Text Analysis

TF-IDF was used to transform textual reviews into numerical features.

### VADER Analysis

VADER was used to calculate compound sentiment scores and classify reviews as positive, neutral, or negative.

### Category-Level Analysis

Sentiment counts were analysed across app categories to understand differences in user feedback.

---

## 💡 Key Findings

The analysis provides the following insights:

- User reviews can be transformed into numerical features using TF-IDF for machine learning.
- Both Naive Bayes and Logistic Regression can be used for sentiment classification.
- Model evaluation helps compare the performance of different classification approaches.
- VADER provides a simple rule-based approach for classifying review sentiment.
- The compound score provides an overall indication of the sentiment expressed in a review.
- Sentiment varies across different app categories.
- Positive, neutral, and negative reviews can be compared to understand overall user perception.
- WordCloud visualisation helps identify commonly occurring terms in user reviews.

Detailed numerical results, model outputs, and category-wise sentiment counts are available in the Jupyter Notebook.

---

## 📁 Project Structure

```text
Level1-Task4-Sentiment-Analysis/
│
├── README.md
├── Sentiment_Analysis.ipynb
└── dataset.csv

