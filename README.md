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

Prophet
Arima
Pycaret stacking
LSTM 

![Models](Images/First_comparizon_time_series.png)

By now the best model for ETH seems to be Arima, but for other cryptos like Swipe that is more 
volatile and has less data the accuracy and predictions turns very bad 24/07/2020

