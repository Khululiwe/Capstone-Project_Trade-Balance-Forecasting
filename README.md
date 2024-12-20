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

Data cleaning and filtering were critical to preparing the dataset for analysis. This process involved:

- Standardizing Column Names: Renaming columns to ensure consistency and ease of processing.
- Handling Missing Values: Addressing missing data by imputing values or removing rows/columns where necessary.
- Outlier Detection: Identifying and treating outliers to reduce their impact on analysis.
- Filtering Relevant Data: Retaining only essential features for meaningful insights and removing noise.

## 6. Exploratory Data Analysis (EDA)

Exploratory Data Analysis (EDA) offered comprehensive insights into the structure and relationships within South Africa's trade balance and GDP data. Key findings and steps included:

- Distribution Analysis: Histograms and box plots highlighted the distribution of trade balances and GDP. The trade balance data exhibited a left-skewed distribution, with most values clustering near zero but with significant deficits for certain trading partners.

- GDP Analysis

  - Summary Statistics: GDP data (2004–2023) showed steady growth, with notable turning points in 2011, 2017, and 2021.
  - Trends Visualization: A line plot revealed GDP’s upward trajectory over two decades.

- Correlation Analysis: Relationships among variables, such as trade balances across partners and years, were explored using scatter plots and correlation matrices.

- Outlier Detection: Outliers were identified using the interquartile range (IQR) method, with 1,633 outliers detected across trade balances. Key contributors included the "World" partner (total of all partners) and "Area NES" (miscellaneous regions).
  Positive and negative outliers totaled 773 and 860, respectively.

- Trade Partner Analysis: Histograms and average balance calculations revealed that South Africa's trade data is predominantly stable, with a few extreme deficits and surpluses.
  The "World" partner’s trade balance aligned with the total of all trading partners, confirming its comprehensive nature.

- Trend Analysis: Top & Bottom Trading Partners: Bar plots identified the top 5 partners with the highest surpluses and the bottom 5 with the largest deficits.

- Absolute Balances: Partners with the most significant absolute trade balances were visualized to highlight both surpluses and deficits.

- Country-Level Comparisons: Comparisons across countries and regions highlighted key trading trends, outliers, and potential areas for economic improvement.
  The left-skewed trade balance distribution emphasized reliance on imports from specific partners, signaling areas requiring policy focus for sustainable growth.

## 7. Modelling

Various statistical and machine learning models were used to analyze and predict trade balance and GDP trends. Key approaches included:

- Linear Regression: Establishing baseline relationships between variables.
- Time Series Forecasting: Using models like ARIMA to predict future trends based on historical data.

## 8. Final Model

The final model(s) were selected based on robust evaluation processes:

Optimization of Parameters: Fine-tuning hyperparameters for better accuracy and predictive power.
Validation: Using cross-validation techniques to ensure model generalization to unseen data.
Evaluation Metrics: Models were assessed using R-squared, mean squared error (MSE), and other performance metrics.

The selected model(s) demonstrated strong performance in explaining the variance in GDP and trade balance data and making reliable forecasts.

## 9. Conclusion and Future Work

This project underscores the critical role of clean data and advanced models in understanding economic trends and making accurate forecasts.
The analysis of trade balance and GDP data has provided valuable insights into economic dependencies and potential future trajectories.

Future Work:

- Dynamic Updates: Incorporate real-time data to enable up-to-date forecasting and improve decision-making.

- Advanced Econometric Models: Explore models like VAR (Vector Autoregression) and structural equation modeling for multivariate time-series analysis.

- Scenario Analysis: Develop simulations to assess the impact of global events (e.g., economic sanctions, trade agreements) on trade balance and GDP trends.

- Interactive Visualization: Build user-friendly dashboards that allow stakeholders to interactively explore the data, forecasts, and insights for better engagement and communication.

- By addressing these future work items, the project can achieve greater scalability and provide more impactful tools for economic analysis.

## 10. References

- World Bank Open Data: https://data.worldbank.org
- OECD Economic Indicators: https://data.oecd.org
- Introduction to Econometrics by James H. Stock and Mark W. Watson
