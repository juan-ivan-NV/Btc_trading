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

## First attempt

![Models](Images/First_comparizon_time_series.png)

Arima performed best predictions but I will keep trying with different models and hyperparamenters

## Second attempt 

* Prophet: hyperparameter changepoint_prior_scale=1.1 - best MSE

![FbProphet](Images/prophet1.png)

* XGBoost: Working on it.

* Arima: 

* Pycaret blender 3 models:
![PyCaret](Images/Pycaret_blender3.png)

* LSTM: Working on it

Comparing again PyCaret, FbProphet and ARIMA for ETH forecasting (Last 40 days)

![comparizon](Images/comp3.png)

* GRU: Working on it.





