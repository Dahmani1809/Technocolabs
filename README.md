>#  TECHNOCOLABS
---
>## Predicting Volatility in Equity Markets Using Macroeconomic News
<p></p>
<p></p>

 ### **PROBLEM STATEMENT**
---
**INTRODUCTION**
<p>In this project, we investigate how macroeconomic sentiment immediately impacts the volatility in liquid markets, by measuring market volatility through the VIX  (volatility index of the S&P 500). Using data pulled from Twitter, we are researching how breaking economic news affects the markets, and subsequently how to predict which news stories can increase volatility. We will consider a tweet ’significant’, in that the news presented in the tweet contributes to volatility in the market, if within 30 minutes of the tweet being tweeted, the volatility of the asset increases by one-fifth of a standard deviation.</p>

**TYPE OF PROBLEM**
<p>On June 26, 2015, months of debt negotiation between the Greek government, headed by Prime Minister Alexis Tsipras, and its creditors, including the IMF and fellow Eurozone countries, broke off abruptly. Tsipras announced a snap referendum regarding the terms of the pending bailout. By the following morning, S&P500 was down significantly.  As political and economic uncertainty grew in Europe, investors across the world were moving their funds away from risky assets that could be negatively affected by a Greek default, and towards safer assets. Days later, when the Greek situation had ’resolved’, the process reversed as equities rallied.</p>
<p>These market movements are not uncommon; just weeks later, crisis erupted in the Chinese equity markets, and asset values were responding to the uncertainty this provoked. </p>

***TYPE OF MACHINE LEARNING PROBLEM - Regression problem***

***METRICS USED - Root mean squared error, r2_score, mean absolute error***
**MODELLING**

1.	LINEAR REGRESSION

* Root mean squared error:  3.21915272492018
* Mean absolute error: 2.0020878617333757
* R2_ score: 0.9997137803863846

2. 	RANDOM FOREST REGRESSOR

* Root mean squared error:  3.7323628408837366
* Mean absolute error:  1.541480477827273
* The r2_score:  0.9996152452921067

3.	DECISION TREE REGRESSOR

* Root mean squared error:  5.458927755021028
* Mean absolute error:  1.9165530876627683
* The r2_score:  0.9991769410872122

4. XGBOOST

* Root mean squared error:  4.966387324197614
* Mean absolute error:  1.7910139818093553
* The r2_score:  0.999318764294927

5. GRADIENT BOOSTING REGRESSOR

* Root mean squared error:  4.418906056666085
* Mean absolute error:  1.6720831283440263
* The r2_score:  0.9994606809432487

<p>From the analysis and comparing all the models, Linear Regression model performs best on the dataset. </p>


**DEPLOYMENT**

Heroku application [Click here](https://volatility-prediction.herokuapp.com/ "click here")

