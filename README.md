Working on it ...

# Stage 1 Data extraction

Much data to feed models is very good because if it's too much data for one model you can try with one more model for example if we could get millions of data then it would be better try with a neural network with data by minute or try a reinforcement learning model.


    Option 1: Obtaining data by day scrapping.

    Option 2: Connect to an API and get limited requests to obtain prices or pay (I don't want to pay).

    Option 3: Look for databases or files with data for free.

    Option 4: Create a boot to capture data by minute of any criptocurrenci for free.

For me the best option is option 1 but the model will not be good if we want to trade by short periods like hours, so the best one is option 4 but is not as easy as it sounds, anyway i will try a bot with selenium to request data by minute.

1.- Scrapping data from: https://coinmarketcap.com/

2.- You can get data by hour from ... but only till each monday of each week:

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



![Models](Images/First_comparizon_time_series.png)

By now the best model for ETH seems to be Arima, but for other cryptos like Swipe that is more 
volatile and has less data the accuracy and predictions turns very bad 24/07/2020

Example of Full_Analizer_Arima(Tuned)_ETH near date 26/07/2020.

![Arima-ETH](Images/high_vs_forecast.png)

After date 26/07/2020.
![Arima-ETH](Images/arima_eth_6preds.png)


Best model is arima tuned for XMR, ETH and BTC with data by day but there are some issues with dates format.