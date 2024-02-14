Project 4 Stock Prediction ML

Team Members:
- Nicholas Mukensnabl
- Kaelan Purcell
- Eric Green

  
Goal: Predict whether a stock price will be up or down in the future using historical stock market data and machine 
learning.

Summary:
- Data Source: Yahoo Finance
- Database = Spark
- Model = RandomForestClassifier

1. Downloaded weekly historical stock price data for SPY & VIX from Yahoo Finance in the form of CSVs.
2. Imported those CSVs into a Spark database.
3. Converted the Spark DataFrames into Pandas DataFrames for easier cleaning.
4. Merged, cleaned, and prepped the data to be used in our RandomForestClassifier model.
5. Trained the model and got a precision accuracy score of 0.61538...
6. Imported another CSV file with historical price data for the 10-year treasury bond (TNX).
7. Prepped the TNX data and then merged it with the existing DataFrame.
8. Retrained the new model with the TNX data and decreased the accuracy score to 0.61404...
9. Added Lag & SMA predictor columns to increase model accuracy score to 0.72222...
10. Removed the 10-year treasury bond (TNX) from the predictors and score remained at 0.72222...
11. Removed VIX from the predictors and score increased to 0.77777...
12. Plotted SPY (Adj Close), VIX and TNX to show how the prices move over the legnth of the analysis.



Sources:
https://www.geeksforgeeks.org/python-pandas-dataframe-reset_index/?ref=lbp
https://www.geeksforgeeks.org/how-to-calculate-moving-averages-in-python/
https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
https://www.w3schools.com/python/pandas/ref_df_floordiv.asp#:~:text=The%20floordiv()%20method%20divides,the%20values%20of%20the%20DataFrame.
https://saturncloud.io/blog/converting-a-column-to-date-format-in-pandas-dataframe/#:~:text=Method%201%3A%20Using%20the%20to_datetime,to%20a%20standard%20datetime%20format.
https://www.freecodecamp.org/news/how-to-rename-a-column-in-pandas/
https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html
https://www.youtube.com/watch?v=1O_BenficgE&list=LL&index=11
https://www.youtube.com/watch?v=CbTU92pbDKw&list=LL&index=10
