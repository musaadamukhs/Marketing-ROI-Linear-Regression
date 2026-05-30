 Marketing-ROI-Linear-Regression
 Marketing ROI Analysis using Simple Linear Regression

Project Overview
This project analyzes a marketing dataset to determine which advertising channel (TV, Radio, or Social Media) yields the highest correlation with Sales. A Simple Linear Regression model was built using `statsmodels` to calculate the Return on Investment (ROI) and provide a data-driven budget recommendation.

 Environment Setup
To run this project locally or in a notebook environment, install the following required Python libraries:
```bash
pip install pandas numpy matplotlib seaborn statsmodels scipy

.
Key Findings

1. Feature Selection & Correlation
After conducting Exploratory Data Analysis (EDA) and computing a Pearson correlation matrix, TV advertising emerged as the single strongest predictor of Sales by a massive margin:
TV to Sales Correlation: 0.9995 (Near-perfect positive linear relationship)
Radio to Sales Correlation: 0.8686 (Strong positive relationship)
Social Media to Sales Correlation: 0.5274 (Moderate positive relationship)

 2. Model Performance & Statistical Significance
A Simple Linear Regression model was fitted using Ordinary Least Squares (OLS) with **TV** as the independent variable ($X$) and Sales as the dependent variable ($y$). 

R-squared ($R^2$): 0.999
    Interpretation: This means exactly 99.9% of the variance in Sales data is explained by the variation in the TV marketing budget alone. This indicates an exceptionally strong, near-perfect model fit.
P-value:< 0.001 (`0.000` in the OLS table)
    Interpretation: The relationship is highly statistically significant. The probability that this strong relationship occurred by pure chance is virtually zero.

 3. Return on Investment (ROI) Coefficient
TV Coefficient ($\beta_1$): 3.5615    Interpretation: For every $1.00 increase in the TV advertising budget, product Sales are predicted to increase by an average of $3.56 (assuming all other factors remain constant). This represents a highly lucrative, predictable return on ad spend (ROAS).
Intercept ($\beta_0$ / `const`): -0.1325 (with a p-value of 0.188)
    Interpretation: Theoretically, this is the baseline sales value if TV spend drops to zero. However, because its p-value is greater than 0.05 (0.188), this negative intercept is not statistically significant from zero, meaning baseline sales with no TV spend are essentially negligible.

---

 Strategic Business Recommendation
Based on empirical evidence, the company should **prioritize and aggressively maximize allocation toward the TV advertising channel. 

While Radio also shows a strong correlation (0.8686), TV dominates the data with an unparalleled linear predictability of 0.9995 and an exceptional R-squared of 0.999. Every single dollar shifted from other channels into TV yields a reliable **$3.56 return in sales**. We recommend shifting underperforming budgets away from Social Media and directly into TV to maximize overall sales revenue in the upcoming fiscal quarters.
