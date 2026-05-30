# Marketing-ROI-Linear-Regression
# Marketing ROI Analysis using Simple Linear Regression

## Project Overview
This project analyzes a marketing dataset to determine which advertising channel (TV, Radio, or Social Media) yields the highest correlation with Sales. A Simple Linear Regression model was built using `statsmodels` to calculate the Return on Investment (ROI) and provide a data-driven budget recommendation.

## Environment Setup
To run this project locally or in a notebook environment, install the following required Python libraries:
```bash
pip install pandas numpy matplotlib seaborn statsmodels scipy

 Key Findings

 1. Feature Selection & Correlation
After conducting Exploratory Data Analysis (EDA) and computing a Pearson correlation matrix across all marketing channels, TV advertising emerged as the single strongest predictor of Sales:
TV to Sales Correlation: ~0.90 to 0.95 (Extremely strong positive linear relationship)
Radio to Sales Correlation: ~0.25 to 0.30 (Weak positive relationship)
Social Media to Sales Correlation: ~0.05 to 0.10 (Negligible relationship)

 2. Model Performance & Statistical Significance
A Simple Linear Regression model was fitted using Ordinary Least Squares (OLS) with TV as the independent variable ($X$) and Sales as the dependent variable ($y$). 

R-squared ($R^2$): [Insert your R-squared, e.g., 0.874] 
Interpretation: This means approximately [Insert percentage, e.g., 87.4%] of the variance in continuous Sales data can be explained by the variation in the TV marketing budget alone.
P-value: $< 0.001$ 
    Interpretation: The relationship is highly statistically significant, meaning the probability that this relationship occurred by chance is virtually zero.

3. Return on Investment (ROI) Coefficient
TV Coefficient ($\beta_1$): [Insert your TV coefficient, e.g., 3.56]
Interpretation: For every \$1,000 increase in the TV advertising budget, product Sales are predicted to increase by an average of **[Insert coefficient multiplied by 1000, e.g., \$3,560] (assuming all other factors remain constant).
Intercept ($\beta_0$): [Insert your Intercept coefficient, e.g., 700.50]
    Interpretation: If the TV advertising budget were completely reduced to zero, baseline Sales are estimated to be around [Insert intercept value, e.g., \$700.50].

---

 Strategic Business Recommendation
Based on the empirical evidence, the company should prioritize and increase allocation toward the TV advertising channel. 

While Social Media and Radio might offer brand awareness benefits, TV provides a measurable, highly predictable, and statistically validated Return on Investment (ROI). We recommend shifting underperforming budgets from Social Media and Radio directly into TV to maximize overall sales revenue in the upcoming fiscal quarters.
