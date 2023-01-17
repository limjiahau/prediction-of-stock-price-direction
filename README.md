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
Date	Open	High	Low	Close	Adj Close	Volume
0	1997-05-15	2.437500	2.500000	1.927083	1.958333	1.958333	72156000
1	1997-05-16	1.968750	1.979167	1.708333	1.729167	1.729167	14700000
2	1997-05-19	1.760417	1.770833	1.625000	1.708333	1.708333	6106800
3	1997-05-20	1.729167	1.750000	1.635417	1.635417	1.635417	5467200
4	1997-05-21	1.635417	1.645833	1.375000	1.427083	1.427083	18853200
...	...	...	...	...	...	...	...
4776	2016-05-09	673.950012	686.979980	671.409973	679.750000	679.750000	3982200
4777	2016-05-10	694.000000	704.549988	693.500000	703.070007	703.070007	6105600
4778	2016-05-11	705.789978	719.000000	701.650024	713.229980	713.229980	7338200
4779	2016-05-12	717.380005	722.450012	711.510010	717.929993	717.929993	5048200
4780	2016-05-13	714.640015	719.250000	706.510010	709.919983	709.919983	4763400
4781 rows × 7 columns
