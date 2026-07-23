# Modeling Volatility and Risk Spillover Between the Financial Markets of US and China Using GARCH Value-at-Risk Forecasting and Granger Causality

[![Thesis DOI](https://img.shields.io/badge/Thesis%20DOI-10.5281%2Fzenodo.21507695-blue)](https://doi.org/10.5281/zenodo.21507695)
[![Code DOI](https://img.shields.io/badge/Code%20DOI-10.5281%2Fzenodo.21506848-blue)](https://doi.org/10.5281/zenodo.21506848)

Undergraduate thesis, Department of Economics, Seoul National University (June 2020).
**[Read the thesis](https://github.com/MajorLift/volatility-modeling-python-datasci/blob/master/Thesis.pdf)** · **[Analysis notebook](https://github.com/MajorLift/volatility-modeling-python-datasci/blob/master/Thesis_code.ipynb)**

*Editorially revised 2026: byline, numeric presentation, and prose. Results, methods, figures, and findings are unchanged from the submitted version.*

> **Keywords**: VaR(Value at Risk), ARIMA-GARCH model, Risk management

## Motivation

Comparative analysis of international economies during two periods of elevated volatility: the Great Recession of 2008 and the Coronavirus Recession. The chosen window captures both against the backdrop of a sustained bull market, allowing the two downturns to be compared directly rather than each against a quiet baseline.

## Dataset

Intraday returns (January 2007 - April 2020)
- S&P500
- SSE Composite Index
- Chinese Yuan to USD exchange rate
> Source: Yahoo Finance

## Libraries

NumPy · Pandas · Statsmodels · SciPy · Seaborn · Matplotlib

## Methodology

- Volatility Forecasting:
  - **Skewed Student’s t ARIMA-GARCH model**
    - Augmented Dickey-Fuller Test for Stationarity
    - Jarque-Bera Test of Normality
    - Box-Ljung Test of Autocorrelation
    - Breusch-Pagan Test for Heteroskedasticity
  - **Parametric Value-at-Risk (VaR)**
- Risk Spillover: **Granger Causality**

## Results

The ARIMA-GARCH VaR estimates fit the historical series closely, with failure ratios meeting the well-specified threshold at both the 5% and 1% confidence levels across most asset and date-range combinations. The Coronavirus Recession is the exception: the short window and unprecedented volatility together degrade forecast performance.

Risk spillover between the two economies is substantial across the full range, but **its predictive power markedly diminishes during both recessions** — that is, precisely when a spillover signal would be most useful, it is least reliable.

## Repository contents

| Path | Contents |
|---|---|
| `Thesis.pdf` | The thesis (25pp) |
| `Thesis_code.ipynb` | Primary analysis notebook — data prep, model fitting, VaR estimation, Granger tests |
| `Thesis_code.html` | Rendered notebook, viewable without Jupyter |
| `jupyter_notebooks/` | Working notebooks: ARIMA order selection by AIC, model summaries, raw dataset |

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

## Citation

```
Suh, Jongsun (2020). Modelling Volatility and Risk Spillover Between the Financial
Markets of US and China Using GARCH Value-at-Risk Forecasting and Granger Causality.
Undergraduate thesis, Department of Economics, Seoul National University.
https://doi.org/10.5281/zenodo.21507695
```

ORCID: [0009-0003-5053-4246](https://orcid.org/0009-0003-5053-4246)

The thesis and the analysis code are archived separately: the DOI above cites the thesis; [10.5281/zenodo.21506848](https://doi.org/10.5281/zenodo.21506848) cites this repository.
