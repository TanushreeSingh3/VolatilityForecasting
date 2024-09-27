
# Volatility Forecasting using ARCH and GARCH Models

## Overview
This project analyzes and forecasts the volatility of the SPY ETF (S&P 500 ETF) using ARCH and GARCH models. The analysis includes downloading historical price data, calculating daily returns, and visualizing both daily returns and simulated volatility series. The project utilizes the `arch` library for modeling, and `yfinance` for data acquisition.

## Table of Contents
- [Installation](#installation)
- [Data](#data)
- [Analysis](#analysis)
- [Results](#results)
- [Dependencies](#dependencies)
- [License](#license)

## Installation
To run this project, ensure you have Python installed along with the required libraries. You can install the necessary packages using pip:

pip install numpy pandas yfinance arch matplotlib

## Data
The project fetches historical price data for the SPY ETF from Yahoo Finance starting from January 1, 2005, to May 30, 2024. The data includes adjusted closing prices, which are used to calculate daily returns.

## Analysis
The analysis consists of the following steps:
1. **Data Loading**: Download historical price data using the `yfinance` library.
2. **Daily Returns Calculation**: Calculate daily returns in percentage.
3. **Volatility Calculation**: Compute daily, monthly, and annual volatility from daily returns.
4. **GARCH Modeling**:
   - Simulate ARCH(1) and GARCH(1,1) series.
   - Fit GARCH models to the daily returns.
   - Forecast future volatility using the fitted models.
   - Compare volatility forecasts from ARCH, GARCH, and EGARCH models.

## Results
- **Daily Returns Visualization**: Plots the daily returns of the SPY ETF.
- **Simulated Volatility Plots**: Visualizes the simulated variances of ARCH and GARCH models.
- **Fitted Model Summary**: Outputs a summary of the fitted GARCH model, including coefficient estimates and statistics.
- **Volatility Forecasts**: Displays forecasted variance for the next 5 days.

### Example Outputs
- Daily volatility: `x%`
- Monthly volatility: `x%`
- Annual volatility: `x%`
- GARCH Model Summary
- Volatility forecasts plot showing forecasts from different models.

## Dependencies
This project requires the following Python libraries:
- `numpy`
- `pandas`
- `yfinance`
- `arch`
- `matplotlib`

