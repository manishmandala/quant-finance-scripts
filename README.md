# Quant Finance Scripts

Small standalone scripts exploring portfolio theory and risk analysis,
written for a finance/investing club. Not packaged as a full app - just
focused scripts that pull real market data and produce real analysis.

## Project2.py - Efficient Frontier / Max Sharpe Ratio

Simulates 10,000 random portfolios across five stocks (AAPL, MSFT, GOOG,
AMZN, JPM), computing expected return, volatility, and Sharpe ratio for
each, then plots the efficient frontier and highlights the portfolio with
the best risk-adjusted return.

## RiskTester.py - Return, Volatility & Correlation Analysis

Pulls historical prices for a set of tickers, computes annualized expected
return and volatility for each, and plots a correlation heatmap between
them - a quick way to see how diversified (or not) a set of holdings
actually is.

## Run it

```bash
pip install -r requirements.txt
python Project2.py
python RiskTester.py
```

Both scripts download live data via `yfinance`, so they need an internet
connection and will reflect whatever the market's doing when you run them.
