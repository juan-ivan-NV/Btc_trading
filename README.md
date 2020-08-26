Working on it ...

# Stage 1 Data extraction

The methods I used to extract data

    1.- Scrapping data from: https://coinmarketcap.com/ 

![Coins](Images/coinsav.png)

![Coins](Images/typecoin.png)

![Coins](Images/rangesgraph.png)


Script at: https://www.kaggle.com/jinuezb/cryptocurrencies-daily-data
    
    2.- Also It's possible to get data by hours or days from https://www.cryptodatadownload.com/data/ but only till each Monday of each week.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Stage 2 Time series forecasting
First attempt

![Models](Images/First_comparizon_time_series.png)

Arima performed best predictions but I will keep trying with different models and hyperparamenters

Second attempt with: 
* Prophet: hyperparameter changepoint_prior_scale=1.1 - best MSE

![FbProphet](Images/prophet1.png)

* Arima: 

* Pycaret 3 models: 

* LSTM: Working on it



