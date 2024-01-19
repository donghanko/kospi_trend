# KospiTrend-Forecasting
In this work, let $x_t$ be the stochastic process of stock prices. We define the trend (momentum) as $\bf{Simple\ Moving\ Average}$. 

$$ SMA_t = E(x_t,n) = \frac{x_t+\cdots +x_{t-n+1}}{n}$$

Based on Geometric Brownian Motion (GBM) : 

$$ \frac{dX_t}{X_t} = \mu_t dt + \sigma_t dW_t,$$

we wish our returns to be distributed near the $\mu_t$ in order to grant for the construction of the momentum. Since the returns of stock prices are assumed to be disturbed by the volatility terms, we need a filtering process to build a forecasting model of the trend. The filtering method of the forecasting model in this project is chosen to be a $\bf{Kalman\ Filter}$.

The Kalman Filter requires two prerequisites equations: [1] the transition equation and [2] the measurement equation. Within this filtering method, we build a trend forecasting model based on one-Dimensional Convolutional Neural Network (1D-CNN) model. 

We compare 1D-CNN prediction model with Kalman Filtered time series as input data with other neural network and settings in terms of time series metrics. 

