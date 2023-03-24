# AutoRegression
Autoregression is a **time series model** that uses observations from previous time steps 
as input to a regression equation to predict the value at the next time step. It is a very 
simple idea that can result in accurate forecasts on a range of time series problems.

$$y_t = c + \phi_1 y_{t-1} + \phi_2 y_{t-2} + ... + \phi_p y_{t-p} + \epsilon $$

$\epsilon$ is the error term of the equation
