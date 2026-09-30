# Air Liquide Quantitative Analysis

Quantitative equity analysis of Air Liquide (`AI.PA`) relative to the CAC 40 index, developed for the GEM Finance Society.

The project studies historical performance, volatility, drawdowns, tail risk and simulation-based return scenarios using market data from 2010 to 2024.

## Overview

Air Liquide is a French multinational company providing industrial gases and services to sectors such as healthcare, chemicals and electronics. It is a major component of the CAC 40 index.

The analysis compares Air Liquide with the CAC 40 to support an investment discussion based on risk-adjusted performance and downside-risk metrics.

## Analysis Components

### Data Collection and Preparation

- Historical price data retrieved with `yfinance`
- Time frame: January 2010 to December 2024
- Comparison between Air Liquide (`AI.PA`) and CAC 40 (`^FCHI`)
- Data cleaning and alignment of market time series

### Performance Analysis

- Cumulative performance indexed to base 100
- Comparative performance versus the CAC 40
- Return and volatility visualization

### Statistical Metrics

- Annualized geometric mean return
- Annualized volatility
- Sharpe ratio, with a zero risk-free rate assumption
- Correlation between Air Liquide and CAC 40 returns

### Monte Carlo Simulation

- 10,000 simulated return paths
- Simulation based on the historical return distribution
- Investment horizons of 1, 5, 10 and 15 years
- Visualization of simulated terminal returns

### Risk Assessment

- Maximum drawdown
- Value at Risk (VaR) at 95% confidence
- Conditional Value at Risk (CVaR)
- Probability of exceeding a 20% drawdown

## Tech Stack

- Python
- pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- yfinance

## Scope

This project is an educational equity-analysis notebook. It is intended to support a structured investment discussion, not to provide investment advice or a production-grade valuation model.
