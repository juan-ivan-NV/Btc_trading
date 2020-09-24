
# Welcome to this project

In this script I've been triying to get the best forecastings as possible trying with different time series models.

Whole script at: https://www.kaggle.com/jinuezb/cryptocurrencies-daily-data

Credits to:



----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Stage 1 Data extraction


The methods I used to extract data

    1.- Scrapping data from: https://coinmarketcap.com/ 

![Coins](Images/coinmkp_1.png)

* Showing firsts 200 coins available:

![Coins](Images/coinsav_2.png)

* Coins names:

![Coins](Images/allcoins_3.png)

* Graph ethereum high price since source firsts recordings

![Coins](Images/coinbehave_4.png)
    
    2.- Also It's possible to get data by hours or days from https://www.cryptodatadownload.com/data/ but only till each Monday of each week.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Stage 2 Time series forecasting


## First model Prophet 

Prophet perform better to forecastings for seasonal data 

![Models](Images/prophet_5.png)






