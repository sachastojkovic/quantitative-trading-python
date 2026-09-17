# Quantitative Trading Strategy : Nasdaq-100 Momentum

## Overview

This project develops and evaluates a simple quantitative trading strategy based on the 50-day moving average of the QQQ ETF, which tracks the Nasdaq-100.

The objective is to explore how a systematic trading strategy performs compared to a traditional buy-and-hold investment.

This project was developed using Python as an introduction to quantitative finance and algorithmic trading.

## Objectives

- Retrieve historical financial market data.
- Calculate daily returns and moving averages.
- Develop a simple momentum trading strategy.
- Backtest the strategy using historical data.
- Compare its performance with a buy-and-hold benchmark.
- Analyze risk-adjusted performance.

## Methodology

The strategy uses a 50-day moving average (MA50) as a trading signal.

### Trading rules

- If the QQQ price is above its 50-day moving average, the strategy holds the asset.
- If the QQQ price is below or equal to its 50-day moving average, the strategy stays in cash.
- The trading signal is shifted by one day to avoid using information from the same day's closing price.

The strategy is compared against a buy-and-hold investment in QQQ.

## Performance Metrics

The following metrics are used to evaluate the strategies:

- Total return
- Annualized volatility
- Sharpe ratio
- Maximum drawdown

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- yfinance
- Google Colab

## Project Structure

```text
quantitative-trading-python/
│
├── Nasdaq100_Momentum_Strategy.ipynb
└── README.md
```

## Key Findings

The notebook compares the performance and risk characteristics of the momentum strategy and the buy-and-hold benchmark.

Results and conclusions are based on the historical backtest presented in the notebook.

## Limitations

This project is intended for educational purposes.

The backtest does not necessarily account for:

- Transaction costs
- Taxes
- Slippage
- Market impact
- Out-of-sample validation
- Changing market conditions

Past performance does not guarantee future results.

## Results
| Metric | Buy & Hold | Momentum MA50 |
| Total Return | 533.35% | 231.08% |
| Annualized Volatility | 22.09% | 13.92% |
| Sharpe Ratio | 0.89 | 0.87 |
| Maximum Drawdown | -35.12% | -18.87% |

## Disclaimer

This project is not investment advice. It is an educational project designed to explore quantitative trading concepts using Python.

## Author

Sacha Stojkovic

BSc in Economics and Finance + Magistère Economist Engineer 
Aix-Marseille School of Economics — AMSE
