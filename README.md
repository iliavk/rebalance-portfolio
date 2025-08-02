# Portfolio Rebalancing Strategies: A Comparative Analysis

## Overview

This project evaluates the performance of several portfolio rebalancing strategies using historical data from two ETFs:

- **SPY**: Represents the S&P 500 index (stocks)
- **BIL**: A short-term U.S. Treasury ETF (proxy for T-Bills)

The baseline allocation is 30% in T-Bills (risk-free asset) and 70% in the equity index. The strategies are backtested from 2010 to 2024.

## Strategies Implemented

1. **Daily Rebalancing** – Reset allocation to 30/70 every trading day.
2. **Monthly Rebalancing** – Reset allocation on the first trading day of each month.
3. **Buy & Hold** – Allocate once at the beginning and never rebalance.
4. **Threshold Rebalancing** – Rebalance only when the actual weights drift beyond a fixed threshold (e.g., 3%, 5%, 10%).

Transaction costs of 0.05% per rebalance are included in the simulation.

## Performance Evaluation

We evaluate all six rebalancing strategies based on four key metrics:
- **CAGR (Compound Annual Growth Rate)**
- **Volatility**
- **Sharpe Ratio** (Assuming 5% risk-free rate)
- **Max Drawdown**

| Strategy           | CAGR   | Volatility | Sharpe Ratio | Max Drawdown |
|--------------------|--------|------------|---------------|---------------|
| Daily              | 10.01% | 12.14%     | 41.24%        | -24.49%       |
| Monthly            | 9.99%  | 12.01%     | 41.51%        | -24.09%       |
| Buy & Hold         | 11.49% | 14.66%     | 44.24%        | -29.99%       |
| Threshold (3%)     | 10.14% | 12.16%     | 42.28%        | -24.48%       |
| Threshold (5%)     | 10.02% | 12.24%     | 41.03%        | -25.09%       |
| Threshold (10%)    | 10.32% | 12.25%     | 43.47%        | -24.67%       |

**Interpretation:**
- **Buy & Hold** shows the highest CAGR, but also the highest drawdown and volatility.
- **Threshold (10%)** offers the best Sharpe ratio among the rebalancing strategies.
- **Monthly and Threshold (3%)** offer a good compromise between return and risk.
- **Daily rebalancing** does not offer significant benefit and could be inefficient with transaction costs.

Note: These results assume a constant transaction cost of 0.05% per rebalance. No variations in cost were explored in this version.

