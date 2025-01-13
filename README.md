## Business Problem
NIFTY 50 is a market index calculated by the National Stock Exchange (NSE) of India, consisting of 50 prominent stocks listed on the exchange. The index value is derived based on the weighted average of the free-float market capitalization of these stocks. Predicting the overall increase or decrease in NIFTY prices has been a challenging task for brokers, as various economic and market factors impact the movement of the index.

## Aim
The goal of this project is to identify the key factors that influence NIFTY price fluctuations and develop a predictive model that can forecast whether the NIFTY index will increase or decrease. This model will provide brokers with valuable insights to guide their customers and make more informed decisions in the stock market.

## Data Needed
The key data needed to build this predictive model includes:
- Percentage change in NIFTY prices
- Various influencing factors such as:
  - INR to USD exchange rate
  - Bloomberg Commodity Index
  - Indian Crude Oil prices
  - Other macroeconomic indicators
  
All data is represented in percentage values.

## Data Sources
The dataset has been collected from Bloomberg over the past 5 years (every 6 months).

## Kind of Analytics
- **Descriptive Analytics**: To understand and summarize the existing data.
- **Predictive Analytics**: To forecast future trends in NIFTY based on historical data.

## Dataset Overview
- **Size**: 43 rows and 13 columns
- **Attributes**: Mostly numerical
- **Missing Values**: 1 missing entry, which was replaced by the mean value of the respective column.
- **Outliers**: Identified and removed using appropriate techniques.

## Data Preprocessing
1. **Null Values**: Missing data was filled using the mean of the respective column.
2. **Outliers**: Detected using statistical methods and removed to ensure model accuracy.
3. **Duplicates**: No duplicate entries found in the dataset.

## Visualizations
- **Heatmap**: To understand the correlation between different factors and the NIFTY price. Factors with a correlation greater than 0.5 are considered impactful.
- **Regression Plot**: To visualize the relationship between different features and the NIFTY price. A higher R-squared value (above 0.6) indicates a better predictor of NIFTY price.

## Machine Learning Techniques
1. **Classification (Decision Tree Classifier)**:
   - The goal is to predict whether the NIFTY price will increase or decrease based on the given factors. A Decision Tree classifier is used to categorize NIFTY price movements into different brackets rather than predicting exact values due to the lack of certain external factors like Fed Balance Sheet and RBI OBICUS data.
   
2. **Clustering (K-Means)**:
   - K-Means clustering is used to categorize the data into groups with similar characteristics. This helps in identifying the most important factors and reducing the dimensionality of the dataset.
   - It also provides insights into how the data points are distributed and grouped, aiding in the categorization of similar data points for better predictions.

