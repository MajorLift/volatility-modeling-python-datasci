# Modeling Volatility and Risk Spillover Between the Financial Markets of US and China Using GARCH Value-at-Risk Forecasting and Granger Causality

Undergraduate Thesis published by the Seoul National University Department of Economics (2020). (**[Read here](https://github.com/MajorLift/volatility-modeling-python-datasci/blob/master/Thesis.pdf)**)

> **Keywords**: VaR(Value at Risk), ARIMA-GARCH model, Risk management

## Motivation

Comparative analysis of international economies during two periods of elevated volatility: the Great Recession of 2008 and the Coronavirus Recession.

## Dataset

Intraday returns (January 2007 - April 2020)
- S&P500
- SSE Composite Index
- Chinese Yuan to USD exchange rate
> Source: Yahoo Finance

## Libraries

- NumPy
- Pandas
- Statsmodels
- SciPy
- Seaborn
- Matplotlibs

## Methodology

- Volatility Forecasting:
  - **Skewed Student’s t ARIMA-GARCH model**
    - Augmented Dickey-Fuller Test for Stationarity
    - Jarque-Bera Test of Normality
    - Box-Ljung Test of Autocorrelation
    - Breusch-Pagan Test for Heteroskedasticity
  - **Parametric Value-at-Risk (VaR)**
- Risk Spillover: **Granger Causality**

## Conclusion

While a considerable degree of risk spillover is observed between the US and Chinese economies throughout the date range, its predictive power is shown to markedly diminish during the two Recession periods.

## References

- Box, G; Jenkins, G. (1970), “Time Series Analysis: Forecasting and Control”, San Francisco:
Holden-Day.
- Bollerslev, T. (1986), “Generalized Autoregressive Conditional Heteroskedasticity”, Journal of Econometrics, April, 31:3, pp. 307–27.
- Granger, C. W. J. (1969), “Investigating Causal Relations by Econometric Models and Cross- Spectral Methods,” Econometrica 37, 424-438.
- Granger, C.W.J. (1980), “Testing for Causality: A Personal View,” Journal of Economic Dynamics and Control 2, 329-352.
- Hamilton, J.D. (1994), “Time Series Analysis”, Taylor & Francis US.
- Hansen, B. (1994), “Autoregressive Conditional Density Estimation,” International Economic Review 35, 705-730.
- Lee, S. and B. Hansen (1994), “Asymptotic Theory for the GARCH(1,1) Quasi-maximum Likelihood Estimator,” Econometric Theory.
- Morgan, J.P. (1996), “Risk Metrics–Technical Document”, 4rd Edition, Morgan Guaranty Trust Company: New York.
