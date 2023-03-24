<h1 align="center"> AutoRegression </h1>

Autoregression is a **time series model** that uses observations from previous time steps 
as input to a regression equation to predict the value at the next time step. It is a very 
simple idea that can result in accurate forecasts on a range of time series problems.

$$y_t = c + \phi_1 y_{t-1} + \phi_2 y_{t-2} + ... + \phi_p y_{t-p} + \epsilon $$

$\epsilon$ is the error term of the equation

A **constraint** to using auto regression is that the time series data needs to be stationary.

## Stationarity
Stationarity means that:
1. $\mu$ is constant
2. $\sigma$ is constant
3. There is no seasonality

![examples of time series data that violated the above constraints](img/Statinarity.jpg)

### Checking For Stationarity
1. Visually
2. Global vs Local Tests
3. Augmented Dickey Fuller (ADF) 
