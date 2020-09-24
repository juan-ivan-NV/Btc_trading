
# Welcome to this project

In this script, I've been trying to get the best forecastings as possible trying with different time series models.

Whole script at: https://www.kaggle.com/jinuezb/cryptocurrencies-daily-data

Credits to:



----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Stage 1 Data extraction


The methods I used to extract data:

    1.- Scraping data from: https://coinmarketcap.com/ 

![Coins](Images/coinmckp_1.PNG)

* Showing first 200 coins available:

![Coins](Images/coinsav_2.PNG)

* Coins names:

![Coins](Images/allcoins_3.PNG)

* Graph ethereum high price since the source first data:

![Coins](Images/coinbehave_4.PNG)
    
    2.- Also It's possible to get data by hours or days from https://www.cryptodatadownload.com/data/ but only till each Monday of each week.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Stage 2 Time series forecasting


## First model Prophet 

Prophet performs better forecasting for seasonal data but in this case the mse is not that bad.

![Models](Images/prophet_5.PNG)

![Models](Images/prophetmse_6.PNG)

## Second model Arima (Autoregressive integrated moving average)

For more info about the model: https://www.machinelearningplus.com/time-series/arima-model-time-series-forecasting-python/

In this case (dealing with ETH) it's predictions do not fit changes as close as is desired.

![Models](Images/arimamse_7.PNG)

## Third model XGBoost (Extreme Gradient Boosting)

For more info about the model: https://xgboost.readthedocs.io/en/latest/tutorials/model.html

Good performance and fast training time.

![Models](Images/xgbmse_8.PNG)

## Fourth model Pycaret 

For more info about this tool: https://pycaret.org/regression/

In this case is used the function Blend Models: This function creates an ensemble meta-estimator that fits a base regressor on the whole dataset. It then averages the predictions to form a final prediction.

![Models](Images/pycaretmodels_9.PNG)

![Models](Images/pycaretmse_10.PNG)

## Fifth model RNN - LSTM (Long Short Term Memory) 

Some information to understand RNN's https://colah.github.io/posts/2015-08-Understanding-LSTMs/

For forecastings I choose a window size of 20 data, It means that each prediction is done considering the 20 data before and all the weights that the network is saving.

![Models](Images/pycaretmodels_9.PNG)

## Sixth model RNN - GRU (Gated Recurrent Units)

Same workflow as the model ↑ but different RNN model also included in the link provided ↑.

![Models](Images/grumse_12.PNG)

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Stage 3 Comparing forecastings


Data frame with last 20 days high price and forecastings from all models.

![Comparing](Images/finaldf_13.PNG)

![Comparing](Images/finalg_14.PNG)

Finally all mse models is compared showing that pycaret performed the best forecastings followed by XGBoost model.

![Comparing](Images/mse_15.PNG)

# Notes

Results are not always the same, sometimes one model perfoms better than other, for example when I start with first testings ARIMA forecastings fited close to the real price, in this case RNN's are not working as good as desired because the data is not enough to train them.

In next stages I will try forecastings with data by hour and windows of 24 data.