# Air Liquide Quantitative Analysis

## Overview
This repository provides a comprehensive quantitative analysis of Air Liquide (AI.PA) compared to the CAC 40 index. The study covers historical performance, risk metrics, probability of positive returns, and key financial indicators using data from 2010 to 2024.

## Company Background
Air Liquide is a French multinational company providing industrial gases and services to industries such as healthcare, chemicals, and electronics. Founded in 1902, it is a prominent component of the CAC 40 index.

## Analysis Components

### 1. Data Collection & Preparation
- Historical price data retrieved using Yahoo Finance API (`yfinance`)
- Timeframe: January 1, 2010 – December 31, 2024
- Compared Air Liquide (AI.PA) with CAC 40 (^FCHI)
- Data cleaning and alignment by removing missing values

### 2. Performance Visualization
- Cumulative performance charts normalized to base 100
- Comparative performance of Air Liquide vs CAC 40
- Volatility and returns visualizations

### 3. Statistical Analysis
Key financial metrics calculated:
- **Geometric Mean Returns** (annualized)
- **Volatility** (annualized standard deviation of returns)
- **Sharpe Ratio** (risk-adjusted returns, risk-free rate = 0)
- **Correlation Matrix** (Air Liquide vs CAC 40 returns)

### 4. Probability & Monte Carlo Simulation
- Monte Carlo simulations: 10,000 paths using historical return distribution
- Statistical probability estimates assuming normal distribution
- Time horizons: 1, 5, 10, 15 years
- Visualizations of simulated end-period returns

### 5. Risk Assessment
- **Maximum Drawdown (MDD)**
- **Value at Risk (VaR)** at 95% confidence
- **Conditional VaR (CVaR)**
- **Drawdown Exceedance Probability** (probability of exceeding 20% drawdown)

## 🛠️ Technical Implementation

### Libraries Used
```python
import matplotlib.pyplot as plt
import seaborn as sns
import yfinance as yf
import pandas as pd
import numpy as np
from scipy.stats import norm
