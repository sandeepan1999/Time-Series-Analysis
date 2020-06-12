# Time Series Forecasting - Project Overview
* Forecasted Retail Sales Time Series using the ARIMA and PROPHET models.
* Preprocessed the dataset and selected relevant features.
* Compared forecasts between two features.

## Code and Resources used
__Python Version:__ 3.7

__Packages:__ pandas, numpy, matplotlib, itertools, statsmodels

__ARIMA Article:__ https://www.digitalocean.com/community/tutorials/a-guide-to-time-series-forecasting-with-arima-in-python-3

__PROPHET Article:__ https://www.digitalocean.com/community/tutorials/a-guide-to-time-series-forecasting-with-prophet-in-python-3

## Data
The dataset used is the Superstore sales data which has 9995 rows and 21 columns.

The column names are:
* Row ID	
* Order ID	
* Order Date	
* Ship Date	
* Ship Mode	
* Customer ID	
* Customer Name	
* Segment	
* Country	
* City	
* State	
* Postal Code	
* Region	
* Product ID	
* Category	
* Sub-Category
* Product Name	
* Sales	
* Quantity	
* Discount	
* Profit

For this project we'll be focusing on the 'Furniture' and 'Office Supplies'.

## Data Preprocessing
This step includes removing columns we do not need, check missing values, aggregate sales by date and so on.

* Dropped all columns except 'Order Date' and 'Sales'.
* Grouped the dataframe by 'Order Date'.
* Resampled the data to use the averages daily sales value for months.

## Data Visualisation
Visualized th data using a method called time-series decomposition that allows us to decompose our time series into three distinct components: trend, seasonality, and noise.

![alt text]

## Model Building
I applied one of the most commonly used method for time-series forecasting, known as ARIMA, which stands for Autoregressive Integrated Moving Average.

ARIMA models are denoted with the notation ARIMA(p, d, q). These three parameters account for seasonality, trend, and noise in data.

I validated the forecasts using Root Mean Square Error(RMSE). I chose RMSE because it is easy to interpret.




