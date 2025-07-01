# ASX DMA Execution Simulator (TWAP/VWAP)

A Python-based simulator designed to emulate institutional trade slicing under TWAP and VWAP strategies, using ASX minute-level data. Benchmarked against live market conditions to evaluate execution cost, timing impact, and slippage,framed around BNP's low-latency, best-execution mandates.

## Project Objective

To build a lightweight Direct Market Access (DMA) engine that compares TWAP vs VWAP execution quality under real-world conditions, supporting cost attribution and live trade diagnostics relevant to BNP’s equity microstructure and execution KPIs.

## Key Features

- **Real-Time Execution Simulation:**  
  Uses minute-level **ASX (VAS ETF)** data to simulate the slicing of a 10,000-share institutional order across TWAP and VWAP schedules.

- **Custom Python Pipeline:**  
  Calculates **unit slippage**, **timing impact**, and **cumulative cost**, benchmarking each strategy against **market close prices**.

- **Interactive Dashboards (Plotly):**  
  Visualizes strategy diagnostics, including cost attribution and time-series execution comparison.

- **Volume-Aware Slicing Logic:**  
  Integrates realistic volume-based trade slicing to minimize market footprint and replicate institutional flow under liquidity constraints.

- **Execution Quality Evaluation:**  
  Demonstrates that VWAP scheduling yields **lower cost variance** in volatile windows, aligned with BNP’s focus on low-impact trade execution.

## Output Metrics

- Execution curves (TWAP vs VWAP)
- Slippage distribution histograms
- Cost decomposition plots
- Market price overlays for benchmarking
