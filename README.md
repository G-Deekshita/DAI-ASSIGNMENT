# DAI-ASSIGNMENT
# Titanic Dataset - Data Cleaning and Exploratory Data Analysis (EDA)

## Overview
This project involves cleaning and exploring the Titanic dataset to uncover patterns and insights about passengers, survival factors, and relationships between features. The workflow includes handling missing values, treating outliers, standardizing data, and performing various statistical and visualization techniques.

## Data Cleaning Steps
1. **Handling Missing Values:**
   - Filled missing values in:
     - `age`: Median value.
     - `fare`: Median value.
     - `embarked`: Mode value.
     - `home.dest`: 'Unknown' placeholder.
   - Dropped columns with excessive missing values: `cabin`, `boat`, `body`.
   - Dropped remaining rows with unfillable missing values.

2. **Duplicate Removal:**
   - Identified and removed duplicate rows to ensure unique records.

3. **Outlier Treatment:**
   - Capped outliers in `age` and `fare` using the IQR method.

4. **Standardizing Categorical Values:**
   - Fixed text inconsistencies in `sex`, `embarked`, `pclass`, and `home.dest`.

## Exploratory Data Analysis (EDA)
1. **Univariate Analysis:**
   - Summary statistics (mean, median, mode, variance, skewness, kurtosis) for numerical variables.
   - Frequency distributions for categorical features.

2. **Visualizations:**
   - Histograms and box plots to understand distributions.
   - Correlation matrix heatmap to detect numerical relationships.
   - Scatter plots for continuous variable interactions.
   - Pair plots for multi-variable comparisons.
   - Bar and violin plots for categorical vs numerical comparisons.
   - Grouped comparisons (e.g., average fare by sex and passenger class).

## Key Findings
- **Survival Insights:**
   - Higher survival rates among females and first-class passengers.
   - Passengers boarding at Cherbourg paid higher fares on average.

- **Age and Fare Distribution:**
   - Fare distribution is highly skewed; some extreme values exist despite capping.
   - Age distribution is more balanced but shows distinct peaks for children and adults.

- **Feature Relationships:**
   - Strong correlation between passenger class and fare.
   - Grouping by sex and class reveals distinct survival and fare patterns.

