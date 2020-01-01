# Stock-Price-Forecasting-and-Visualisation

# Aim
The aim of this final project is two folded:
1. Visualisation of a particular stock using different indicators.
2. Utilisation of various machine learning models to predict the price movement of the stock.

# Content

## 1. Data Collection
- Use Alpha Vantage to fetch live stock data 

## 2. Features Addition
- Add financial indicators like Bollinger Bands, MACD, RSI to the dataframe

## 3. Indicators
- Create gauge charts to measure market sentiment, news sentiment and 52-week range.

Market Sentiment

News Sentiment

52-week Range

## 4. Machine Learning
- Apply two machine learning learning models (Random Forest and LSTM) to predict the stock price movement in 2019 with the usage of 2013-2018 data


### Result
Facebook (Sumbol: FB) is used as the stock example for the stock price prediction. 

#### Random Forest Model
![Random Forest Result](https://github.com/kasparkwok/Stock-Price-Forecasting-and-Visualisation/blob/master/Random_Forest_Price_Prediction.PNG)

As seen from the circled part of the graph, the prediction using random forest is unrealistic as no price changes are recorded for a few days in the prediction. In pursuit of finding a model that can forecast the stock price more accurately, Long-Short Term Memory (LSTM) Model is used instead. 

#### LSTM Model
![LSTM Result](https://github.com/kasparkwok/Stock-Price-Forecasting-and-Visualisation/blob/master/LSTM_Price_Prediction.PNG)
