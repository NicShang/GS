# Algorithmic Execution Efficiency Analysis

This project simulates and evaluates algorithmic trading strategies (TWAP vs. VWAP) using high-frequency execution data, designed to reflect the daily workflow and performance metrics.

## Objective

To analyze the execution efficiency and slippage risks between **TWAP** and **VWAP** strategies under volatile intraday conditions, using **Circle Inc.** trading data (June 24, 2025). 
---

##  Methodology

- **Data**: 1-minute interval OHLCV data from Circle Inc. (2025-06-24).
- **Execution Strategies**: Simulated large-volume orders using both **TWAP** and **VWAP** algorithms.
- **Stress Testing**: Injected market noise via **Monte Carlo simulations** (N=1000) to reflect intraday volatility and execution stress.
- **Benchmarking**:
  - Calculated VWAP benchmark from actual data.
  - Measured slippage as *(execution price - VWAP benchmark)*.
- **Analytics**: 
  - Distribution plots of execution prices and slippage.
  - Mean/Std deviation of slippage.
  - Strategy win-ratio evaluation.

---

## Results Snapshot

- **TWAP Average Slippage**: -1.76  
- **VWAP Average Slippage**: +0.01  
- **Win Ratio**: TWAP outperformed VWAP in **100% of simulations** under stress.

> Interpretation: In this scenario, TWAP provided more consistent execution outcomes with lower risk of adverse slippage, which can inform BNP's algorithm tuning under liquidity stress or volatile listings.
---
