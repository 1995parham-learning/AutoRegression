<h1 align="center"> AutoRegression </h1>

Autoregression is a **time series model** that uses observations from previous time steps 
as input to a regression equation to predict the value at the next time step. It is a very 
simple idea that can result in accurate forecasts on a range of time series problems.

$$y_t = c + \phi_1 y_{t-1} + \phi_2 y_{t-2} + ... + \phi_p y_{t-p} + \epsilon $$

$\epsilon$ is the error term of the equation

A **constraint** to using auto regression is that the time series data needs to be stationary.

## Stationarity (weak)
Stationarity means that:
1. $\mu$ is constant
2. $\sigma$ is constant
3. There is no seasonality

![examples of time series data that violated the above constraints](img/Statinarity.jpg)

### Checking For Stationarity
1. Visually
2. Global vs Local Tests
3. Augmented Dickey Fuller (ADF) 

A very common idea to transform a non-stationary data to a stationary one is differnecing. If $y_t$ is not stationary $y_t - t_{t-1}$ may be stationary.

## Auto Correlation Function (ACF)
Let's explain this by an example:
$S_t$ Average price of Salmon this month
The most intuitive determiner of the price of Salmon this month is the price of Salmon last month and then the month before that and on and on.
![ACF](img/ACF.jpg)
The direct effect may be a big food festival for example which happens every two months and affacts the price of Salmon
