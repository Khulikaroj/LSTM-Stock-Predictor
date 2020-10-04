# LSTM-Stock-Predictor


## Objective
In this assignment, I build and evaluate deep learning models using both the FNG values and simple closing prices to determine if the FNG indicator provides a better signal for cryptocurrencies than the normal closing price data.

Model 1: Use "close price of Bitcoin" as feature input into LSTM RNN model.

Model 2: Use "Fear and Greed Indicator"  as feature input into LSTM RNN model.


## Model Architecture
Sequential model is used. For model architecture and parameters, I compare up to three layers added into the model and compare between different optimizer such as "adam", "rmsprop", and "sgd". Moreover, rolling window size is varied to find the best fit model.  I use adam as optimizer, epoch = 20, and batch size = 1 for common model specification. Then, compare window size between 10, 5, 2 and 1. 

## Findings

1. Model 1 which use closing price as feature always have lower loss compare to Model 2 which us the FNG indicator as input.

2. Model 1 also track the actual data over time better than Model 2.

Model 1
![](Model1.png)

Model2
![](Model2.png)

3. From varying the window size, window size of 2 days work best. 1-day window size has higher loss compared to using 1-day window size and does not work in Model 2.


