## 🔍 Overview
This Jupyter Notebook analyzes how socioeconomic indicators like poverty rate, CPI, utility costs, and CalFresh meal counts drive food bank distribution volumes across California zipcodes. It combines ACS demographic data, BLS CPI, utility costs, CalFresh’s reported meals, and actual food distribution metrics to uncover demand drivers and build a predictive model.

## 🗂️ Data Analysis & Key Plots
- **Socioeconomic Distributions:** Histograms of poverty rate and unemployment highlight skewness and outliers.
- **Correlation Heatmap:** Displays pairwise correlations (e.g., poverty vs. meals, CPI vs. meals) for feature selection.
- **Choropleth Map:** Visualizes meals delivered per capita by zipcode to identify high-demand areas.
- **Scatter Plot:** Meals delivered vs. poverty rate with regression line showing demand dependence.
- **Box Plot:** Meal cost distribution across low-, mid-, and high-income zipcodes to compare variability.
- **Time-Series Line Chart:** Unemployment rate vs. monthly meal volume illustrating a negative trend.

## 🤖 Predictive Modeling
- **Feature Engineering:** Cost-per-meal ratio, poverty-to-population ratio, utility-cost index.
- **Model Training:** Liner Regression, Decision Tree regresison Random Forest regression on train/test split (80/20).
- **Performance:** R² = 0.68, MSE = 6.99 in predicting median income.
- **Evaluation:** Residual analysis and feature importance ranking—poverty rate and CPI are top predictors.

## 🎯 Use Case
A policy analyst or nonprofit manager can:
- Identify which factors (poverty, CPI, utilities) most strongly influence meal demand.  
- Target high-need areas via choropleth and scatter visualizations.  
- Use the income-prediction model to estimate local purchasing power and optimize resource allocation.

## 🛠️ Tech Stack
- **Python 3.10+** & **Jupyter Notebook**  
- 🐼 `pandas`, 🧮 `numpy` for data wrangling  
- 📈 `plotly.express` & 🔍 `seaborn` for interactive & statistical plots  
- 🤖 `scikit-learn` for regression modeling  
