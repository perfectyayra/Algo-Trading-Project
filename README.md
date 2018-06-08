# Algorithm Trading with Machine Learning Methodologies



## Team Members

Perfect Yayra Gidisu  1702010695

Mathilde Bouvier      1702010703

Faruk Yucel           1702010705



```
"Better stock prices direction prediction is a key reference for better trading strategy and decision
making by ordinary investors and financial experts" (Kap, Chiu, Lu and Yang; 2013).
```

## Introduction

Due to increasingly large volume of data, manually analyzing data for some tasks like predicting stock market movements has become impractical if not impossible for humans hence the need for automation. By providing large amount of data, machine learning algorithms explore the data and search for a model that will achieve the programmer’s goal. The objective of our project is to implement momentum strategy using machine learning. We tried to predict trading signals using machine learning techniques based on a set of rules using technical indicators. 

## Methodology

We formulated the problem of stock trading decision as a classification problem with two different classes: buy and sell. The aim of this project is to identification of the most efficient classifier based on some metrics.
We used some momentum and volatility technical indicators with time periods of 7, 14 and 28 days as predictors. Since, some of these indicators may be irrelevant for our data. We used random forest variable importance technique to figure out the insignificant predictors. As a result, we obtained these relevant indicators: Relative Strength Index, Commodity Channel Index, Momentum(for time period=7), William’s %R , Ultimate Oscillator, Rate of Change. These indicators are then standardized to be fed as input in different models.

As usual machine learning can be divided into two stages. First stage is when the model is trained, and a second one, in which the system classifies the data accordingly to the technical indicators trained during the stage one. The result of the analysis is the predicted trend of the market index, which can be used to set out some trading rules:

• If the next day trend is Uptrend, then the decision is BUY

• If BUY decision already exists, then HOLD

• If the next day trend is Downtrend, then the decision is SELL

• If SELL decision already exists, then HOLD

According to the result obtained with these rules, the return of strategy has been calculated.



## Data

We pulled the daily historical data from Morningstar. We chose 4 stocks (BIDU, MSFT, AAPL and TXN) in the technology sector (NDXT index) of the NASDAQ. The time period is from 01/01/2007 to 31/12/2017. The dataset is composed of 6 variables: date, opening price of the day, highest price of the day, lowest price of the day, closing price of the day, traded volume. We used 80% of this data as our training set and 20% as test set.

## Model
We used the following models and an ensemble of these models.
- KNN
- Decision Tree
- Random Forest
- SVM
- Gaussian Naïve Bayes




## Results
We see that our returns are indeed positive and in line with actual market returns eventhough actual returns are slightly higher in some periods.

![](Images/9.png)
![](Images/2.png)
![](Images/6.png)

![](Images/7.png)

Based on the return from our strategy, we do not deviate that much from the actual market return. Indeed, the achieved momentum trading strategy made us well predict the stock prices direction to invest/desinvest in order to make profits. However, as our accuracy is not 100% (but more than 96%) therefore, we made relatively few losses compared to the actual returns. 

## References

- Leung, C.K.S., MacKinnon, R.K. and Wang, Y., 2014, July. A machine learning approach for stock price prediction. In Proceedings of the 18th International Database Engineering & Applications Symposium (pp. 274-277). ACM.
- Madge, S. and Bhatt, S., 2015. Predicting Stock Price Direction using Support Vector Machines. Independent Work Report Spring.
- Teixeira, L.A. and De Oliveira, A.L.I., 2010. A method for automatic stock trading combining technical analysis and nearest neighbor classification. Expert systems with applications, 37(10), pp.6885-6890.
- https://www.tradingtechnologies.com/help/x-study/technical-indicator-definitions
