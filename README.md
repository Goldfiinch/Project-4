Project 4 Stock Prediction ML

Team Members:
- Nicholas Mukensnabl
- Kaelan Purcell
- Eric Green

  
Goal: Predict future stock prices using historical stock market data and machine 
learning.


Summary:
- API = Yahoo Finance
- Database = Spark
- Model = Neural Network LSTM (Kera’s Bi-Directional Model)

- 
Using the Yahoo Finance API, we will import historical stock data for a single stock 
into the Spark database. Using Pandas, we will then clean the data and prepare for 
use in training a neural network model to predict the chosen stock’s future prices. 
After some preliminary research, we decided to use Kera’s Bi-Directional LSTM 
Model as it is the most common model used for stock market time-series data. 
Because stock market data is commonly viewed in line-chart form, we also plan to 
include some line-charts to better visualize the price predictions. 
