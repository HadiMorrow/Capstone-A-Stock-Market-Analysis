## Problem Statement

While most of us wish to make an easy buck, many do not know where to start. We took the liberty to address this issue by attempting to predict the stock market. Specifically, comparing the aggregate mean of the NASDAQ to two specific big players in the market, AAPL and GOOGL. Collecting stock market data from IEX cloud, we were able to retrieve data over 2 months and 5 years.
Using time series models, RNN and SARIMAX, we will come up with a model that attempts to trace the market. Our goal is to determine the limit to predicting the market in this way and to determine if a more volatile stock like AAPL is predicted better or worse than GOOGL and so on.

## Executive Summary

At the start of this project we were certain we would build a superior model to anything on the market with crude tools and a wild imagination. Come to find that it is not really that easy. Using SARIMAX we were able to come up with am okay but not great start. After venturing down this rabbit hole, an RNN was used. These models appear to be better according to the train test accuracy.

Following this better guess we decided to run all 372 stocks in the same RNN model. After doing so we clustered the results to determine high accuracy clusters. Using 4 clusters we were unable to determine anything significant however after using 11 clusters we were able to determine that high performing models tend to have a larger last price and much more market cap while the exact opposite is true for low accuracy models.

Thus if one was to use RNN to predict stocks and gamble on the market, doing so with large companies would likely yield better results.
For future work, we would like to dig into the different clusters. Really dig into other indicators like beta scores, P/E ratio, other indicators and studies which we can implement to see if we can rationally come up with a reason for why or what makes up a good predicting stock model.


## Conclusions

As we conclude this analysis, it is important to notice how computationally heavy this type of work can be. A larger computer should be used next time as well as implementing Bayesian Statistics where we can infer the probability of a binary outcome based on a previous probability prediction.
