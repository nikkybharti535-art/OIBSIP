# Task 4 - Unveiling the Android App Market

## 📌 Project Overview

This project performs a comprehensive analysis of the Google Play Store ecosystem using app data and user reviews.

The analysis covers app categories, ratings, installs, pricing, app size, estimated revenue, and user sentiment.

## 🎯 Objective

- Analyze the Google Play Store app ecosystem.
- Clean and preprocess real-world app data.
- Explore app categories and ratings.
- Analyze installs, size, and pricing.
- Estimate revenue for paid applications.
- Perform sentiment analysis on user reviews.
- Generate data-driven insights for app developers.

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- VADER Sentiment Analysis
- Jupyter Notebook

## 📂 Datasets

Two datasets were used:

1. Google Play Store Apps Dataset
2. Google Play Store User Reviews Dataset

## 🧹 Data Cleaning

The following preprocessing steps were performed:

- Checked missing values.
- Removed duplicate records.
- Converted Reviews into numeric format.
- Converted Installs into numeric format.
- Converted Price into numeric format.
- Converted Last Updated into datetime format.
- Converted app Size into MB.
- Handled missing values.
- Created an Estimated_Revenue feature.
- Removed reviews with missing review text.

### Dataset Information

| Dataset | Original Rows | Duplicates Removed | Remaining Rows |
|---|---:|---:|---:|
| Apps | 10,841 | 483 | 10,358 |
| User Reviews | 64,295 | 33,616 | 30,679 |

## 📊 Exploratory Data Analysis

### 1. Category Analysis

Analyzed the distribution of applications across different categories to identify highly saturated categories.

### 2. Ratings Analysis

Analyzed the distribution of app ratings and calculated the average rating for each category.

### 3. Size vs Installs Analysis

Created a scatter plot to study the relationship between app size and number of installs.

### 4. Pricing Analysis

Compared free and paid applications and analyzed the price distribution of paid applications.

### 5. Revenue Analysis

Estimated revenue for paid applications using app price and installation information.

## 💬 Sentiment Analysis

VADER Sentiment Analysis was used to classify user reviews into:

- Positive
- Neutral
- Negative

Sentiment was also analyzed across different app categories.

## 📈 Visualizations

The project includes:

- App category distribution
- Rating distribution
- Average rating by category
- App size vs installs scatter plot
- Free vs paid app comparison
- Paid app price distribution
- Estimated revenue by category
- Sentiment distribution
- Sentiment by category
- Interactive Plotly visualization

## 🔍 Key Insights

1. FAMILY, GAME, and TOOLS are among the categories with the highest number of applications, indicating strong competition.

2. Free applications greatly outnumber paid applications, showing that the free-download model is more common on the Google Play Store.

3. Positive reviews are generally higher than negative reviews across many categories, indicating generally favorable user experiences.

## 💡 Developer Recommendation

A developer planning to launch a new application should consider market competition, user demand, pricing strategy, and existing user sentiment.

Identifying a specific niche with strong demand and comparatively lower competition may provide better opportunities for growth.

## 📌 Conclusion

This project demonstrates an end-to-end data analytics workflow including data cleaning, exploratory data analysis, visualization, revenue estimation, and sentiment analysis using real-world Google Play Store data.

## 📁 Project Structure

Task-4-Google-Play-Store-Analysis/
│
├── Google_Play_Store_Analysis.ipynb
├── googleplaystore.csv
├── googleplaystore_user_reviews.csv
└── README.md

## 🚀 How to Run

1. Install the required Python libraries.

2. Open the Jupyter Notebook.

3. Place both datasets in the same folder as the notebook.

4. Run the notebook cells sequentially.

## 👩‍💻 Author

Nikky Bharti
