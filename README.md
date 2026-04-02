# Stock Portfolio Optimization using R 📈

## Overview
This project applies **Modern Portfolio Theory (MPT)** to optimize a stock portfolio consisting of four major technology companies: **Apple (AAPL), Microsoft (MSFT), Google (GOOGL), and Amazon (AMZN)**. The optimization is based on historical data from January 2020 to January 2024.

## Objectives
* **Maximize Returns:** Target the best expected mean return for the portfolio.
* **Minimize Risk:** Reduce portfolio variance (risk) using the ROI solver.
* **Real-world Constraints:** Implemented 'Full Investment' (100% allocation) and 'Long-Only' (no short selling) rules.

## Technical Stack
* **Language:** R
* **Libraries:** * `quantmod` - For fetching financial data from Yahoo Finance.
  * `PortfolioAnalytics` - For defining and solving the optimization problem.
  * `PerformanceAnalytics` - For risk and performance metrics.
  * `ROI` (R Optimization Infrastructure) - For numerical optimization.

## Methodology
1. **Data Acquisition:** Adjusted closing prices were pulled using `getSymbols`.
2. **Returns Calculation:** Daily log returns were computed to ensure statistical stationarity.
3. **Optimization:** The portfolio was optimized using the ROI method to find the weights that offer the best risk-adjusted performance.

## Results
The model suggests a strategic concentration in **AAPL (~64%)** and **MSFT (~36%)** to achieve optimal stability for the given period.

![Optimized Weights](optimized_weights.png)

## Author
**A.M.R.N.A. Menike** *BSc (Hons) in Financial Mathematics and Industrial Statistics* University of Ruhuna, Sri Lanka.
