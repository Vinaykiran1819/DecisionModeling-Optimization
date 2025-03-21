# Investing in Stocks - Modern Portfolio Theory

This project focuses on Investing in Stocks and Modern Portfolio Theory (MPT) for Investment and Portfolio Management. The primary goal was to develop and implement an MPT optimization model to select the optimal stock allocations from a set of 9 S&P 500 stocks across multiple sectors. This approach aims to balance risk and return, ensuring portfolio diversification.

## 1. Introduction

Modern Portfolio Theory (MPT) offers a quantitative framework to optimize investment portfolios by balancing expected returns against risk. 

**Why does MPT matter?**

**Risk-Return Balance:** Helps investors find the optimal mix of assets that maximize returns for a given level of risk—or minimize risk for a given return.
**Practical Application:** Used by financial institutions and individual investors alike to make data-driven decisions.

## 2. Project Overview
**1. Data Collection:**

- Gather historical price data for multiple stocks across various sectors.
- Calculate daily or monthly returns to maintain a consistent time series.

**2. Risk & Return Estimation:**

- Compute expected returns (mean returns) and volatility (standard deviation of returns).
- Construct a covariance matrix to capture how stocks move relative to each other.

**3. Optimization Model:**

- Formulate an optimization problem to maximize returns for a target risk or minimize risk for a target return.
- Apply constraints such as total weight = 100% and (optionally) no short selling.

**4. Efficient Frontier & Allocations:**

- Identify the Efficient Frontier, a curve representing the best possible risk-return trade-offs.
- Select a specific portfolio based on criteria (e.g., maximum Sharpe ratio, minimum variance).

**5. Performance Comparison:**

- Compare the optimized portfolio to various rebalancing strategies and a benchmark (e.g., S&P 500).
- Assess metrics like cumulative return, annualized return, and drawdown.

## 3. Results & Visualizations
**3.1 Optimal Stock Allocation for Different Risk Levels**

This chart shows how each stock’s weight shifts as we vary the target risk. Notice that certain stocks dominate at lower risk levels, while higher-risk allocations may favor different stocks with potentially higher returns.

**3.2 The Efficient Frontier**

The Efficient Frontier displays the best possible risk-return combinations. Moving along this curve:

Leftmost Point: Minimum volatility portfolio.
Uppermost Point: Maximum return for a given risk, often associated with a higher Sharpe ratio.

**3.3 Portfolio Performance Comparison**

In this plot, we compare:

Buy-and-Hold vs. Daily, Weekly, and Monthly rebalancing strategies.
Performance is measured by the portfolio’s cumulative return over time.
Rebalancing can help maintain the optimal weight distribution, potentially leading to smoother returns.

**3.4 KDE Plot of Simulated Portfolio Returns**

The Kernel Density Estimate (KDE) illustrates the distribution of simulated annual returns for the portfolio. The dashed red line indicates the expected return, helping visualize where most outcomes cluster around the mean.

# 4. Conclusion
This project underscores how Modern Portfolio Theory can be effectively applied to optimize a portfolio by balancing returns against risk. By leveraging diversification and quantitative optimization techniques, we can systematically allocate assets to achieve desirable risk-return profiles. The visualizations highlight how allocations change with risk preferences and how different rebalancing strategies can affect overall performance.

The model led to an expected 16.81% return over the course of one year, with a 19.2% probability of loss at a 0.0002 risk level. Monte Carlo simulations were used to evaluate various rebalancing strategies, such as daily, weekly, and monthly rebalancing, to assess how frequently the portfolio should be adjusted for optimal performance. This project is a practical application of portfolio management techniques, showcasing how to make informed investment decisions based on risk-adjusted returns.
