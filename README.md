# GLD Trading Strategy

This repository contains a quantitative trading strategy for trading GLD (SPDR Gold Shares) based on moving averages and the Relative Strength Index (RSI). The strategy includes parameter optimization, stop-loss mechanisms, and performance evaluation.

## Overview

The strategy uses the following indicators:
- **9-day moving average**
- **21-day moving average**
- **Relative Strength Index (RSI)**

A trading signal is generated when the short-term moving average crosses the long-term moving average, and it is confirmed by the RSI. A dynamic stop-loss mechanism based on the Average True Range (ATR) is implemented to manage risk.

## Features

- **Data Retrieval**: Downloads historical data for GLD using `yfinance`.
- **Indicators Calculation**: Computes moving averages, RSI, and ATR.
- **Signal Generation**: Generates buy/sell signals based on moving average crossovers and RSI thresholds.
- **Parameter Optimization**: Optimizes the short and long moving average periods and RSI thresholds.
- **Performance Metrics**: Calculates key performance metrics including Sharpe ratio and maximum drawdown.
- **Visualization**: Plots the GLD stock price, moving averages, RSI, and cumulative returns.

## Usage

### Prerequisites

Ensure you have the following Python libraries installed:
- `numpy`
- `pandas`
- `pandas_datareader`
- `matplotlib`
- `yfinance`

You can install these libraries using `pip`:
```bash
pip install numpy pandas pandas_datareader matplotlib yfinance
```
## Running the Code

### 1. Clone the repository:
```bash
git clone https://github.com/yourusername/gld-trading-strategy.git
cd gld-trading-strategy
```
### 2. Run the Python script:
```bash
python gld_trading_strategy.py
```