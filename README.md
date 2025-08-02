# ML_STOCK_PRICE_PREDICTION
This project analyzes historical stock price data for NSE-TATAGLOBAL and builds a regression model using a Random Forest Regressor to predict the 'Turnover (Lacs)'.
Dataset
The dataset used is NSE-TATAGLOBAL11.csv, which contains historical stock data including:

Date
Open Price
High Price
Low Price
Last Price
Close Price
Total Trade Quantity
Turnover (Lacs)
Project Steps
Data Loading and initial exploration: The dataset was loaded into a pandas DataFrame and initial checks were performed to understand its structure, data types, and check for missing values.
Exploratory Data Analysis (EDA):
Calculated descriptive statistics (mean, median, standard deviation, variance) for numerical features.
Examined the date range of the stock data.
Visualized the distribution of 'Close' prices using a histogram.
Plotted 'Close' price over time using a scatter plot.
Analyzed the variation of 'Total Trade Quantity' over time using a line plot.
Investigated the correlation between 'Close' price and 'Total Trade Quantity' using a scatter plot.
Identified potential outliers in numerical columns using a box plot.
Examined the relationship between 'Turnover (Lacs)' and 'Total Trade Quantity' using a scatter plot.
Data Preparation:
The 'Date' and 'Total Trade Quantity' columns were dropped as they were not used as features for predicting 'Turnover (Lacs)'.
The features (X) and target variable (y) were defined.
The data was split into training and testing sets using train_test_split.
Model Training: A Random Forest Regressor model was trained on the training data (X_train, y_train).
Model Evaluation: The trained model's performance was evaluated on the testing data (X_test, y_test) using the Mean Squared Error (MSE) metric.
Feature Importance: The importance of each feature in the trained model was visualized to understand which features contributed most to the prediction of 'Turnover (Lacs)'.
Results
The Mean Squared Error (MSE) of the trained Random Forest Regressor model on the test set was calculated to be {{mse}}. The feature importance plot shows the relative importance of the features in predicting 'Turnover (Lacs)'.
