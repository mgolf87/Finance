# Finance
Repository of different programs for finance and investing
<br />
StochRSI before making an investment to ensure it's a good time to buy or sell - need an abnormal volume detector to buy/sell with
<br />
Supertrend Crypto Trading Bot is key for trading
<br />
Projects all contain code adapted and credited in the notebooks
<br />
<br />

### Stochastic Relative Strength Index - StochRSI
#### StochRSI.ipynb 
Finds if an asset is overbought or oversold via Stochastic RSI
<br />
When a stock goes above 0.8 = good time to sell
<br />
When a stock goes below 0.2 = good time to buy
<br />
<br />
Uses an exponential moving average indicator function (EMA) and a Stochastic RSI function (StochRSI) to plot the closing price and the StochRSI. Oversold (0.2) and Overbought (0.8) lines on the StochRSI graph indicate that when a stock goes above 0.8 it suggests it’s a good time to sell, and when a stock goes below 0.2 it suggests it’s a good time to buy. Comparing the values of the closing prices above and below the overbought and oversold lines indicate whether the decision to sell or buy was correct.

<br />

### Decision Tree Stock Close Price Prediction
#### DecisionTree_StockPrediction.ipynb
Decision tree used to predict if the price of a stock will increase or decrease. Will tomorrows close price be higher or lower than todays close price?

<br />

### Sentiment Analysis for Stock Price Prediction based on Top News Headlines
#### SentimentAnalaysisStockPrice.ipynb
##### (requires upload_DJIA_table.csv; Combined_News_DJIA.csv)
Prediction of price increase or decrease in a stock based on top news headlines. Requires vaderSentiment and textblob installations. Measures sentiment based on the subjectivity and polarity within the news headlines. Subjectivity ranges from 0 (objective) to 1 (subjective) and Polarity ranges from -1 (negative statement) to +1 (positive statement). Sentiment scores are divided into negative, neutral, and positive. The compound score is the score that calculates the sum of all lexicon ratings (normalized between -1 and +1). Linear discriminant analysis was used to make model predictions from the training and test sets. Model resulted in an accuracy of 0.84.

<br />

### Yahoo Finance Trending Ticker Scraper
#### YF_TrendingTickers.ipynb
Program which pulls the trending stock tickers from Yahoo Finance and saves them in a .csv file with the timestamp and trending rank order. Current loop set to fetch the trending tickers every minute and save them into a .csv file.

<br />

### Supertrend Crypto Trading Both
#### SuperTrend_CryptoBot.ipynb
Average True Range (ATR): measure of market volatility via decomposing the entire range of an assest price for that period
<br />
True Range (TR): Max [current high - current low] OR Max [abs(current high - previous close)] OR Max [abs(current low - previous close)] i.e. Max[CH-CL, abs(CH-PC), abs(CL-PC)]
<br />
ATR is just the average of the TR over a specified period
