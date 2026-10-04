# Portfolio Optimization using Monte Carlo Simulation

## Overview

This project explores portfolio construction using **Monte Carlo simulation**. Historical price data for four Indian large-cap stocks is used to simulate 10,000 long-only portfolios and study the relationship between expected return, volatility, and Sharpe ratio.

### Assets
- Reliance Industries (`RELIANCE.NS`)
- TCS (`TCS.NS`)
- Infosys (`INFY.NS`)
- HDFC Bank (`HDFCBANK.NS`)

## Methodology

1. Download approximately two years of historical prices using `yfinance`.
2. Convert prices into daily percentage returns.
3. Estimate mean returns and the covariance matrix.
4. Generate 10,000 random portfolios whose weights sum to 100%.
5. Calculate annualized expected return and volatility.
6. Calculate the Sharpe ratio.
7. Identify:
   - Maximum-Sharpe portfolio
   - Minimum-volatility portfolio
8. Visualize the simulated risk-return opportunity set.

## Key Concepts

The project demonstrates practical use of:

- Portfolio expected return
- Portfolio volatility
- Covariance matrix
- Diversification
- Sharpe ratio
- Monte Carlo simulation
- Risk-return analysis

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- yfinance
- Jupyter Notebook

## Project Structure

```text
portfolio-optimization/
├── portfolio_optimization.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## How to Run

Clone the repository and install the dependencies:

```bash
pip install -r requirements.txt
```

Then launch Jupyter:

```bash
jupyter notebook
```

Open `portfolio_optimization.ipynb` and run the cells from top to bottom.

> `yfinance` retrieves market data from the internet, so an active internet connection is required when running the notebook.

## Important Assumptions & Limitations

- Historical average returns are used as estimates of expected returns.
- The analysis uses 252 trading days for annualization.
- Portfolios are long-only and fully invested.
- No transaction costs, taxes, leverage, or liquidity constraints are modeled.
- The maximum-Sharpe portfolio is the best portfolio found among the 10,000 simulations.

## Disclaimer

This project is for educational and research purposes only and does not constitute investment advice.
