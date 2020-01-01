# Stock-Price-Forecasting-and-Visualisation

# Aim
The aim of this final project is two folded:
1. Visualisation of a particular stock using different indicators.
2. Utilisation of various machine learning models to predict the price movement of the stock.


Facebook (Sumbol: FB) is used as the stock example for both visualisation and stock price prediction. 

# Content

Facebook (Sumbol: FB) is used as the stock example for the stock price prediction. 
## 1. Data Collection
- Use Alpha Vantage to fetch live stock data 

## 2. Features Addition
- Add financial indicators like Bollinger Bands, MACD, RSI to the dataframe

## 3. Indicators
- Create gauge charts to measure market sentiment, news sentiment and 52-week range.

### Market Sentiment
[Relative Strength Index](https://www.investopedia.com/terms/r/rsi.asp)(RSI) is used to measure the recent market sentiment of the stock. 
If the arrow is pointing below 30, that means the underlying stock is oversold. Conversely, if it points above 70, it implies that the underlying stock is overbought.

In the example below, FB is slightly overbought.
![graph](https://github.com/kasparkwok/Stock-Price-Forecasting-and-Visualisation/blob/master/Market_Sentiment.PNG)

### News Sentiment
News and media play an important role for the movement of the stock price. In light of that, I decided to incorporate news sentiment into my visualisation. 
I used [Google News API](https://newsapi.org/s/google-news-api) to fetch news related to the particular company.
To measure the news sentiment of the stock, I used [VaderSentiment](https://github.com/cjhutto/vaderSentiment) to measure whether the relevant news article is perceived as positive, neutral or negative. 
Lastly, I created a gauge chart to display the news sentiment which reflects media's perception about the company for the last 2 days. The gauge chart ranges from -1 (negative) to 1 (positive).  

In the below example, FB is perceived as neutral by the media.
![graph](https://github.com/kasparkwok/Stock-Price-Forecasting-and-Visualisation/blob/master/News_Sentiment.PNG)

### 52-week Range
52 week range shows the lowest price, highest price of last year as well as the current price of the underlying stock. 

In the example below, FB is trading near to its 52-week high price.
![graph](https://github.com/kasparkwok/Stock-Price-Forecasting-and-Visualisation/blob/master/52-Week_Range.PNG)

## 4. Machine Learning
- Apply two machine learning learning models (Random Forest and LSTM) to predict the stock price movement in 2019 with the usage of 2013-2018 data


### Result

#### Random Forest Model
![Random Forest Result](https://github.com/kasparkwok/Stock-Price-Forecasting-and-Visualisation/blob/master/Random_Forest_Price_Prediction.PNG)

As seen from the circled part of the graph, the prediction using random forest is unrealistic as no price changes are recorded for a few days in the prediction. In pursuit of finding a model that can forecast the stock price more accurately, Long-Short Term Memory (LSTM) Model is used instead. 

#### LSTM Model
![LSTM Result](https://github.com/kasparkwok/Stock-Price-Forecasting-and-Visualisation/blob/master/LSTM_Price_Prediction.PNG)
