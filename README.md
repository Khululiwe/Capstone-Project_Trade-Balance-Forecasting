## Capstone Project-Trade Balance & GDP Forecasting

![balance trade](https://github.com/Khululiwe/Capstone-Project_Trade-Balance-Forecasting/blob/main/img/Balance-of-Trade.jpg)

## Table of Contents

- [1. Project Overview](#overview)
- [2. Importing Packages](#packages)
- [3. Data Collection and Description](#data-collection)
- [4. Loading Data](#loading-data)
- [5. Data Cleaning and Filtering](#data-cleaning)
- [6. Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [7. Modelling](#modelling)
- [8. Final Model](#final-model)
- [9. Conclusion and Future Work](#conclusion)
- [10. References](#references)

  ## 1. Project Overview

  #### 1.1. Objective:

To analyze South Africa's trade balance dynamics and its impact on GDP, aiming to identify key trends, build predictive models, and provide data-driven insights for policymakers and businesses.

#### 1.2. Key Tasks:

Time Series Analysis: Identify significant turning points in the trade balance and understand underlying trends.
Correlation Analysis: Determine the relationship between trade balance and GDP.
Machine Learning Modeling: Develop models to forecast future trade balance and GDP.
Policy Implications: Provide actionable insights to optimize economic strategies.

#### 1.3. Hypotheses:

- Null Hypothesis (H₀): There is no significant correlation between changes in the trade balance and GDP.
- Alternative Hypothesis (H₁): There is a significant correlation between changes in the trade balance and GDP.
  <br>

## 2. Importing Packages <a class="anchor" id="packages"></a>

1. Importing Packages:

This section details the libraries imported for data manipulation, visualization, and modeling. These libraries include pandas, numpy, matplotlib, seaborn, statsmodels, scikit-learn, and warnings. The code ensures proper display for large datasets and avoids warnings.

## 3. Data Collection and Description

**Data Source**: The primary trade data comes from Trademap (https://www.trademap.org/), while GDP data is obtained from Statista (https://www.statista.com/statistics/370513/gross-domestic-product-gdp-in-south-africa/).

**Data Description**:
Trading Partners: This dataset focuses on South Africa's trade balance with various partners over 20 years (2004-2023). It includes information on partners and their corresponding yearly trade balance. (File: data/trading-partners.csv, Shape: 235 rows x 21 columns)

GDP: This dataset provides historical and predicted GDP values for South Africa from 1989 to 2029. (File: data/Gross domestic product in South Africa.csv, Shape: 41 rows x 2 columns)

## 4. Loading Data

Both datasets were loaded into pandas DataFrames for further analysis. And the first and/or last few rows of the datasets are previwed, providing details on the data shape and features for each dataset.

## 5. Data Cleaning and Filtering

Data cleaning involves removing noise and irrelevant information from the dataset to improve model accuracy. This includes:

- Standardizing column names
- Handling missing values

## 6. Exploratory Data Analysis (EDA)

EDA helps in understanding the structure of the data and the relationships between different features. Key steps include:

- Visualizing the distribution of categories.
- Examining word frequency distributions.
- Analyzing the length of articles.

## 7. Modelling

Various classification models were trained and evaluated:

- **Logistic Regression**
- **Decision Tree**
- **Random Forest**
- **Support Vector Machine (SVM)**
- **Multinomial Naive Bayes**

## 8. Final Model

Grid search was used to fine-tune hyperparameters and improve model performance. Performance metrics such as accuracy, precision, recall, and F1-score were used to evaluate and compare models.

## 9. Conclusion and Future Work

The automated news classification system effectively categorizes news articles into predefined categories, improving operational efficiency and user experience.

## 10. References

- Continuously update the model with new data to maintain accuracy.
- Explore advanced NLP techniques like BERT for improved performance.
- Integrate user feedback to refine and enhance the classification system.
