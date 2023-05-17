# Bitcoin Price Prediction using Twitter Sentiment Analysis
## Abstract:
Cryptocurrencies are rising in importance as an investment option and alternative currency. Thus, investors are keen on finding timely market movement insights. One such source is Twitter due to its live feed of information on cryptocurrencies and emotional information from investors expressing their sentiments. This article examines the extent to which Twitter sentiments can be used to predict price and transaction volume changes for the nine largest cryptocurrencies for the period of June 2021 to September 2021. This study was conducted using a lexicon-based approach through the VADER algorithm for sentiment analysis, while applying the Granger causality method to analyze the two-way predictive capabilities of each cryptocurrency’s sentiments toward their respective price and transaction volume changes. Past studies have shown that sentiment analysis may work for several cryptocurrencies, while this study only found predictive capabilities in transaction volume changes and not in price movement.
## Abstract:
Cryptocurrencies are digital currencies that utilize blockchain technology (Nakamoto, 2008). There are numerous coins available in the market with the largest one being Bitcoin (CoinMarketCap, 2021). Due to its fairly young age, the cryptocurrency market lacks regulation to govern it (Alexander & Heck, 2020). Lack of regulation, news, and information found on social media is considered the main cause of volatility in the cryptocurrency market (Mai et al., 2018).

A social media platform most commonly used by the investors is Twitter due to its rapid nature and emphasis on the microblogs dissemination, or tweets, which can capture investors' fleeting sentiments (Kraaijeveld & De Smedt, 2020). Coincidentally, previous research has discussed the usage of Twitter, specifically from sentiments found in users’ tweets, to be a method of prediction in the stock market (Bollen et al., 2011; Kraaijeveld & De Smedt, 2020; Li et al., 2018).
## Literature Review
Past studies have explored the usage of algorithms to determine sentiments found in texts. Hutto and Gilbert (2014) tested several sentiment analysis algorithms on social media and found that the best algorithm for sentiment analysis in social media is the VADER algorithm. Unlike other similar lexicon-based algorithms, VADER was created specifically with social media in mind.

A similar study investigating Twitter sentiments using VADER and its effect on the cryptocurrency market was conducted by Kraaijeveld and De Smedt (2020), but it used data from 2018. At the time, the cryptocurrency market capitalization was USD 813 Bn, while the market cap in mid-2021 was USD 1,493 Bn (CoinMarketCap, 2021). The significant increase in capital flow into the cryptocurrency market can be credited to its rising popularity among retail investors, but more importantly, institutional investors have started adding cryptocurrencies into their balance sheets as early as 2019 (Sun et al., 2021). The entry of institutional investors into the cryptocurrency market and the corresponding increase in market size indicate the market has a vastly different landscape today than in 2018. Hence, this necessitates an updated study on Twitter sentiment analysis for investors in the cryptocurrency market.

Based on the aforementioned introduction, there are two objectives to this study, i.e., firstly, it is to investigate whether Twitter sentiments can predict price and transaction volume changes. Secondly, to investigate whether price and transaction volume changes can predict Twitter sentiments.
## Literature Review
This study was conducted using daily data from 1st June 2021 until 30th September 30th, 2021. During the study period, up to 1,000 tweets mentioning the nine largest cryptocurrency tokens by market capitalizationwere collected. Daily prices and the trading volume for each cryptocurrency were collected from CoinMarketCap, a platform for financial information regarding cryptocurrencies. The list of tokens used in this study were Bitcoin (BTC), Ethereum (ETH), Binance Coin (BNB), Cardano (ADA), Dogecoin (DOGE), Rip-ple (XRP), Polkadot (DOT), Uniswap (UNI), and Chainlink (LINK).

In order to make the tweets suitable for use with the VADER algorithm, each raw tweet data obtained was cleaned to remove retweets, hyperlinks, mentions, hashtags, and other symbols. Tweets with terms such as “giveaways” and “giving” were also removed because a previous study by Kraaijeveld and De Smedt (2020) mentioned that cryptocurrency-related tweets generally have a number of bot-made tweets in them, using those exact terms.

Afterward, the cleaned tweet data was fed into the VADER algorithm to measure their polarity and compound score. The tweet was categorized as positive if the compound score was over 0, negative if the compound score was under 0, or neutral if the compound score was 0. The price and transaction volume changes were calculated using a simple return formula.

Three methods were employed for further analysis. First, the Augmented Dickey-Fuller (ADF) test was used to determine the stationarity of the time-series data used in this research. (Dickey & Fuller, 1979). Second, the Johansen Cointegration test was employed to determine if the time-series used in this research were cointegrated, showing whether there exists a long-term connection between them (Johansen, 1988). Lastly, the Granger causality was utilized to see a two-way relationship between two variables, showing whether a certain factor was capable of predicting another factor, or vice versa (Engle & Granger, 1987).

## Conclusion:
In conclusion, the results of the study do not show any significant relationships between Twitter sentiments and price changes. However, a significant result was observed in the predictive capability of sentiment to predict transaction volume changes for BTC, DOGE, DOT, and XRP. Conversely, the results indicate that volume changes have the capabilities of predicting sentiment changes for ADA and DOGE.

These results differ from the previous study on Twitter sentiment analysis and the cryptocurrency market. The discrepancy could be caused by the different market conditions, indicating that retail investors in Twitter no longer have significant influence over price changes in the cryptocurrency market. Furthermore, this could be due to the significant presence of institutional investors, who can be regarded as more rational than retail investors, as they tend to hold their investment positions despite the price and volume fluctuations (Sun et al., 2021).

The results of this study might benefit traders and institutional investors for research focused on the latest analysis of trading strategies using Twitter sentiment analysis. Future research might benefit from implementing supervised machine learning to enhance predictive capabilities for more advanced trading strategies.
## Technologies:
* Programming Languages: Python, Java
* Big data technologies: Spark ML, Spark-SQL, Hadoop Mapreduce
* Libraries: Pandas, Matplotlib, Scikit-learn, TensorFlow , Keras

## Data Used in this Project can be found at this link
https://www.dropbox.com/s/oy5zcf4aiorr0dr/Archive.zip?dl=0

## References:
* http://dataconomy.com/2014/07/bitcoin-big-data-can-predict-future-value-virtual-currency
* http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.375.4517&rep=rep1&type=pdf
* https://arxiv.org/pdf/1610.09225.pdf
