# Algorithm Trading with Machine Learning Methodologies



## Team Members

Perfect Yayra Gidisu  1702010695

Mathilde Bouvier      1702010703

Faruk Yucel           1702010705


## Introduction
```
"Better stock prices direction prediction is a key reference for better trading strategy and decision
making by ordinary investors and financial experts" (Kap, Chiu, Lu and Yang; 2013).
```

## Objective

Our project aims to implement a momentum strategy based on Machine Learning methods. The data consists of Date, Open, High, Low, Last and Volume. We calculated our predictors based on various technical indicators i.e. Exponential Moving Average, Stochastic Oscillator %K and %D, Relative Strength Index (RSI), Rate Of Change (ROC), Momentum (MOM) on which model was trained in order to forecast the direction of stock price. The predictions are used to build a momentum strategy that buy/sell when the next predicted price is above/below the last closing price.

## Feature Selection

Exponential Moving Average (= exponentially weighted moving average) = similar to the simple moving average however more weight is given to the latest data resulting in a faster reaction to recent price changes.

Stochastic Oscillator %K and %D = momentum indicator that compare, over a certain period of time, the closing price of a security to the range of its prices. 
```
Where %K = 100(C - L14) / (H14 - L14)
C = the most recent closing price
L = the low of the 14 previous trading sessions
H14 = the highest price traded during the same 14-day period
%K= the current market rate for the currency pair
%D = 3-period moving average of %K
```

Relative Strength Index (RSI) = momentum indicator that compare, over a certain period of time, the magnitude of recent gains and losses to measure speed and change of price movements of a security.
```
Where: RSI = 100 - 100 / (1 + RS)
RS = Average gain of up/loss of down periods during the specified time frame.
```

Rate Of Change (ROC) = ratio between a change in one variable relative to a corresponding change in another.

Momentum (MOM) = rate of acceleration of a security's price or volume. It is an oscillator and is used to help identify trend lines.

## Data

We pulled the daily historical data from Morningstar. We chose 4 stocks (BIDU, MSFT, AAPL and TXN) in the technology sector of the NASDAQ. The time period is from 01/01/12 to 31/12/17.

## Model

We realized the following methods:
- KNN
- Decision Tree
- Random Forest
- SVM
- Gaussian Naïve Bayes

## Results

