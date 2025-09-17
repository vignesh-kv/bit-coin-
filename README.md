Bitcoin Price Prediction using Machine Learning
Overview
This project predicts whether a Bitcoin trade will be profitable the next day using historical price data (OHLC: Open, High, Low, Close).
The model uses Machine Learning algorithms to analyze trends and provide a buy/sell signal.

Dataset
Source: Bitcoin historical data from 17th July 2014 to 29th December 2022
Columns: Date, Open, High, Low, Close, Volume
Rows: 2713
Features & Target
Engineered Features:
open-close → difference between Open and Close price
low-high → difference between Low and High price
is_quarter_end → 1 if month is Mar/Jun/Sep/Dec, else 0
Target:
target → 1 if next day’s Close price > today’s Close price, else 0
Exploratory Data Analysis (EDA)
Line plots of closing price trends
Histograms & boxplots for price distributions and outliers
Year-wise barplots of average prices
Pie chart for target distribution
Heatmap for feature correlations
Models Used
Logistic Regression
Support Vector Machine (SVM)
XGBoost Classifier
Evaluation:
ROC-AUC score on training and validation sets
Confusion matrix visualization
Results
XGBoost achieved highest training accuracy but showed slight overfitting
Logistic Regression gave a balanced performance on training and validation data
