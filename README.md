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
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 4781 entries, 0 to 4780
Data columns (total 7 columns):
 #   Column     Non-Null Count  Dtype  
---  ------     --------------  -----  
 0   Date       4781 non-null   object 
 1   Open       4781 non-null   float64
 2   High       4781 non-null   float64
 3   Low        4781 non-null   float64
 4   Close      4781 non-null   float64
 5   Adj Close  4781 non-null   float64
 6   Volume     4781 non-null   int64  
dtypes: float64(5), int64(1), object(1)
memory usage: 261.6+ KB
