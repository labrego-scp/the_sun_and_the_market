# Sunspot Activity and Stock Market Returns

## Overview
This repository contains an empirical study testing whether solar activity, measured by sunspot numbers, has predictive power over U.S. equity market returns. The analysis focuses on the S&P 500 index and follows a strictly lagged framework to avoid look-ahead bias.

The goal is not to confirm a prior belief, but to evaluate the statistical and economic relevance of a widely debated hypothesis in behavioral finance.

---

## Data
- **Market data:** Daily S&P 500 prices (`^GSPC`) obtained via `yfinance`.
- **Exogenous data:** Monthly Sunspot Numbers from a public and reputable source (SIDC / SILSO).

Daily returns are aggregated to a monthly frequency to match the availability of the sunspot data.

---

## Methodology
1. Align daily market returns with monthly sunspot observations.
2. Apply a one-month lag to sunspot data to ensure proper timing and prevent look-ahead bias.
3. Conduct exploratory data analysis to assess distributions and outliers.
4. Estimate a baseline predictive model using OLS regression.
5. Evaluate both statistical significance and economic relevance.

---

## Results
- The estimated relationship between lagged sunspot activity and S&P 500 returns is not statistically significant at conventional levels.
- The model explains approximately 0.8% of the variance in returns.
- Confidence intervals include zero and economically negligible effect sizes.

Overall, the results provide no evidence of economically meaningful predictive power.

---

## Investment Interpretation
Based strictly on the empirical results, this signal would not justify capital allocation. Any apparent relationship is consistent with noise rather than a tradable effect.

---

## Requirements
Main Python dependencies:
- pandas
- numpy
- statsmodels
- yfinance
- matplotlib / seaborn

All analysis can be reproduced by running the notebook.
