## Oncology-Data-Exploration

This repository contains code for analyzing oncology data using the `datascience` Python package, which comes from the Computational and Inferential Thinking book by UC Berkeley. The goal of this analysis is to explore relationships between various socioeconomic factors (such as education and poverty levels) and health-related outcomes (such as uninsured health rates), as well as perform basic linear regression, residual analysis, and classification.

The dataset used in this project is `OncologyData.csv`, which can be found at the following link:
https://gist.githubusercontent.com/caterinaponti/08485044a1ba5b5c93000d1875ecacba/raw/75329a5a80ff4779bc1417a1c4a0f440a8459305/OncologyData.csv

The dataset comes from the Women in Data Science 2024 Datathon Challgenge launched in 2024: https://www.kaggle.com/competitions/widsdatathon2024-challenge2/data.

**Dependencies**

To run the analysis, you will need the following Python packages:

- `datascience`: A package that provides simple and efficient tools for exploratory data analysis. It is used widely in UC Berkeley's data science course (Computational and Inferential Thinking).
- `numpy`: For numerical computations.
- `matplotlib`: For plotting graphs.
- `scipy`: For statistical functions.


**Code Overview**

**Regression Analysis**
The script defines several functions to fit and evaluate linear regression models:

Standard Units Calculation: Converts a column of values into standard units.
Correlation: Calculates the correlation between two variables.
Slope and Intercept: Computes the slope and intercept of the regression line.
Scatter Plot with Fit Line: Visualizes scatter plots of variables with the fitted regression line.
Predictive Models
Using nearest-neighbor predictions, the project predicts values for:

Health Uninsured: Based on education levels.
Median Income: Based on high school education levels.
Unemployment Rates: Based on education less than high school.
Residuals and Error Estimation

**Functions are implemented to:**

Calculate residuals (errors) between actual and predicted values.
Visualize residual plots to analyze the goodness of fit.
Bootstrap Resampling
The script performs bootstrap resampling to estimate the variability in the slope of the regression line and computes the 95% confidence interval.

**Classification Task**
A k-nearest neighbor classification model is built to predict whether a patient will be diagnosed within 90 days based on educational and healthcare variables.

**Key Functions**

- `correlation`: Returns the correlation coefficient between two variables.
- `slope`: Computes the slope of the regression line.
- `intercept`: Calculates the intercept of the regression line.
- `fit`: Generates the regression line for given data.
- `scatter_fit`: Visualizes the scatter plot and the regression line.
- `predict_health`, `predict_income`, `predict_unemployement`: Functions for making predictions based on different variables.
- `residual_plot`: Generates a residual plot for analyzing prediction errors.
- `bootstrap`: Performs bootstrap resampling to generate a distribution of slopes and computes the 95% confidence interval.
