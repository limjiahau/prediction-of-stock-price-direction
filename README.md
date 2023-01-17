# Prediction of Stock Price Direction
## Assignment
Predict the day price direction of Amazon.com, Inc. (AMZN) stock.

To be profitable, we need to predict the price direction of the stock: whether it will be higher or lower than the price today. 

The target would be a binary classification whether the next day closing price will be higher than the opening price.

## Data Description
Data from 1997 up to 2020 that has been split into training (1997-2016), validation (2016-2018), and testing (2018-2020) periods. The data is available in AMZN_train.csv, AMZN_val.csv, and AMZN_test.csv files respectively.

Each dataset has the same format with the following 7 columns:
- `Date` - in format `YYYY-MM-DD`
- `Open` - stock price upon opening of an exchange
- `High` - the highest stock price on a given day
- `Low` - the lowest stock price on a given day
- `Close` - stock price at the end of a trading day
- `Adj Close` - adjusted closing price that takes into account corporate actions
- `Volume` - the amount of shares traded over the course of a trading day

# Data Exploration
![image](https://user-images.githubusercontent.com/65124287/212928234-18f0d3de-12fc-4c22-a671-c156b21aed38.png)

![image](https://user-images.githubusercontent.com/65124287/212928946-e9990e27-bceb-4bf6-ac8a-48291b3377c1.png)

Mostly numerical columns (5 floats, 1 int) and an object column for Date. No null values.

Let's plot the stock price as a function of time by:
- passing the Date column as an argument for the x-axis and the
- closing, opening, highest and lowest price for the y-axis.

![image](https://user-images.githubusercontent.com/65124287/212928481-05768f68-69ae-4545-a22c-be1720fec3e4.png)
