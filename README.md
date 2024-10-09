#### *This project conducts an analysis of customer data and uses machine learning to categorize customers. The objective is to uncover insights about their behaviors and spending habits, which can inform better marketing tactics and product development.*

## Table of Contents
1. Introduction
2. Dataset Description
3. Data Cleaning
4. Feature Engineering
5. Exploratory Data Analysis (EDA)
6. Customer Segmentation
7. Conclusion

## Introduction
Customer segmentation helps businesses understand their customers by grouping them into distinct categories. This project analyzes customer data to identify key groups based on their demographics and spending behavior.

## Dataset Description
The dataset includes various customer information, such as:

- Customer ID
- Age
- Gender
- Income
- Spending Score
- Product Category, etc

## Data Cleaning
Before conducting EDA, the following steps were taken to ensure data quality:

1. Handling Missing Values: Checked for missing values and imputed where necessary.
2. Outlier Detection and Removal: Identified outliers in critical variables (e.g., income, age) and removed them to ensure a clean dataset.
3. Data Type Adjustments: Converted columns like Customer ID to categorical where appropriate to avoid skewing results in analysis.
4. Duplicate Records: Scanned for and removed duplicate entries to prevent data bias.



These variables are used to explore trends and create meaningful customer segments.

## Feature Engineering
Feature engineering was performed to create more meaningful insights for the analysis:

- Creating New Features: Based on existing data, we introduced features such as:
    - Income per Product Category: This feature was calculated to understand spending tendencies across various income groups.
    - Age Grouping: Age ranges were binned into categories (e.g., 18-25, 26-35) to observe patterns across age groups.
- Scaling Features: Numerical features like income and spending score were scaled using StandardScaler for clustering analysis.

## Exploratory Data Analysis
The EDA revealed important insights about the customer base:

1. Demographics: Age and income distribution show diverse groups.
2. Spending Patterns: High-income customers tend to spend more, with some notable outliers.
3. Correlations: A strong positive correlation between income and total spending.
4. Product Preferences: Customers in different income groups show varied preferences for product categories.

## Key Visualizations
- Correlation heatmap between numeric variables.
- Distribution plots of income, spending, and age.
- Product spending across different customer groups.

## Customer Segmentation
Using K-Means clustering, we identified three major customer segments:

- Segment 1: Low Income, Low Spend
- Segment 2: Middle Income, Moderate Spend
- Segment 3: High Income, High Spend

Visualizations of the clusters show clear distinctions between these groups, particularly in their spending behavior and income levels.

## Conclusion
The analysis provided actionable insights into customer behaviors. Segmenting customers allows businesses to target their marketing strategies effectively. Further, identifying high-value customers offers the potential to increase revenue through personalized services.

## Usage
### Requirements
- Python 3.x
- Jupyter Notebook
- Libraries: pandas, numpy, matplotlib, seaborn, sklearn
