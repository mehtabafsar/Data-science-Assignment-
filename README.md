# Data-science-Assignment-
Overview
This project is focused on building machine learning models to predict the overall rating of beers based on various features such as beer characteristics, user reviews, and beer styles. The program implements three machine learning models: Random Forest Regressor, Linear Regression, and Gradient Boosting Regressor, and evaluates their performance on predicting the beer ratings.

The goal of the project is to predict the beer rating (review/overall) based on several input features such as the beer's alcohol content, aroma, appearance, and user-provided review text.

Dataset
The dataset used contains the following features:

beer/ABV: Alcohol by volume of the beer.
beer/style: The style or type of beer (e.g., Lager, IPA).
review/appearance: The rating of the beer's appearance.
review/aroma: The rating of the beer's aroma.
review/palate: The rating of the beer's palate.
review/taste: The rating of the beer's taste.
review/text: The user-provided text review.
Target Variable:
review/overall: The overall rating of the beer (1.0 to 5.0).
Feature Engineering:
The review/text column is processed using TF-IDF vectorization, converting the text into numerical features to capture the relevant information.
The beer/style is encoded into numerical values to handle categorical data.
The other numeric columns are scaled using StandardScaler to ensure uniformity in the range of values.
Models Implemented
Three models were implemented and evaluated in this project:

1. Random Forest Regressor
A powerful ensemble model that builds multiple decision trees and averages their results to make predictions. It’s robust and handles non-linear relationships effectively.

2. Linear Regression
A simple and interpretable model that assumes a linear relationship between input features and the target variable. It's quick to train and useful for baseline comparisons.

3. Gradient Boosting Regressor
An advanced ensemble model that builds decision trees sequentially, each one correcting the errors of the previous one. This model tends to perform well in structured data scenarios and can capture complex patterns.

Results
The performance of the models was evaluated using three metrics:

Mean Absolute Error (MAE): Measures the average magnitude of errors in predictions.
Root Mean Squared Error (RMSE): Penalizes larger errors more than MAE.
R² Score: Indicates the proportion of variance explained by the model (closer to 1 is better).
Here are the results for each model:

Random Forest Regressor:
MAE: 0.3010
RMSE: 0.3943
R² Score: 0.6839
Linear Regression:
MAE: 0.2981
RMSE: 0.3908
R² Score: 0.6896
Gradient Boosting Regressor:
MAE: 0.2960
RMSE: 0.3886
R² Score: 0.6930
Model Comparison:
While Gradient Boosting performed the best in terms of all three metrics, both Linear Regression and Random Forest also produced competitive results. Gradient Boosting's ability to capture complex relationships led to slightly better performance, but all models explained a significant amount of variance in the data.
