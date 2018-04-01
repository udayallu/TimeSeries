# TimeSeries
Time Series Analysis using R
https://www.youtube.com/watch?v=wNB8AgZPFLU

## WHY TIME SERIES 
- In Time series we only deal with the **one Variable** that will dependent on the **Time**
- Where as other algorithms such as the **Logistics Regression or Linear Regression** they deal with the **2 Variables** they are **dependent** and the **independent** variables.

## What is Time Series 
- A time series is a series of the data points indexed in timed oreder.
- Most commanly the Time series is a sequence taken at successive equally spaced points in time.
- Time series Forecasting is the use of model to predict future values based on previously observed values.

## When Not  to use the time series 
- when the  values are constant.
- If the data is non stationary.

## What is Stationary 
- The mean shoud be constant according to the time.
- The Variance should be equall at differnt time intervals.
- The co-variance should also be equall

## Components of the Time Series 
1. General Trend
2. Seasonal
3. Irreguar Fluctuations

1. **General Trend** - A General Direction in which the trend is changing.
[]
2. **Seasonal** - A peak or dip which is sean in the time interval.
3. **Iregular Fluctutation** -  The un controlled situtation which aries due to which the value change.
Eg: Flights cancelled due to Fog

## Timeseries models 
### ARIMA
- **AR** - Auto Regression(p)
- **MA** - Moving Average(q)
- **I** - Integration(d)
- we needto get the p,q,d values from the ACF Graph
- ACF means Auto co-relation function graph
```
acf(diff(log(AirPassengers))) # Determines the value of the q
pacf(diff(log(AirPassengers))) # Determines the value of the p
 the p and q value are by default 1, they change on how many times you to differanation 

```

