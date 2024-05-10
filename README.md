# AdEase Wikipedia Page View Forecasting 
Optimized Ad Placement for Ad Ease

This project investigates historical Wikipedia page view data to forecast future views and optimize ad placement for AdEase clients.

## Project Overview
AdEase, an advertising platform, aims to predict page views to strategically place ads for clients across different regions and languages. This project utilizes historical view data for 145,000 Wikipedia pages over 550 days.

## Data Description
The project utilizes two CSV files:

Contains daily page views for each Wikipedia page for 550 days. Each row represents a page, and each column represents a day. The data includes:

Specific Name: Title of the Wikipedia page
Language: Page language (e.g., en.wikipedia.org for English)
Access Type: Device used to access the page (e.g., desktop, mobile)
Access Origin: Source of the request (e.g., browser, web crawler)
Exog_Campaign_eng.csv: Contains a binary flag indicating dates with significant events (campaigns) that might influence page views. This data is only available for English pages (en.wikipedia.org).

## Project Structure
The project consists of Python scripts:

Perform initial data exploration, analyzing structure, missing values, and page name format.
Preprocesses data, including extracting information from page names and handling missing values.
Analyzes time series characteristics for stationarity and visualization.
Implements ARIMA model for forecasting, including stationarity checks and hyperparameter tuning.
Implements SARIMA model with exogenous variables for English pages using the campaign data.
Implements Facebook Prophet for forecasting.
Evaluates and compares model performance using MAPE.
Analyzes results across languages and provides recommendations for ad placement.



## Outcome
Time Series Forecasts: Implementation of ARIMA, SARIMA, and Prophet models to forecast future page views for different languages.
Model Comparison: Evaluation of model performance using MAPE to identify the most suitable approach for each language.
Actionable Insights and Recommendations: Analysis of results and recommendations for optimal ad placement based on predicted page views across different languages.
