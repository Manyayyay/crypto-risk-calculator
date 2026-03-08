# crypto-risk-calculator
crypto-risk-calculator using MCMC
This project analyzes the volatility (risk) of cryptocurrencies using Bayesian MCMC. The goal is to estimate the volatility of individual assets and evaluate the risk of an equal-weight cryptocurrency portfolio.The analysis uses historical price data to compute log returns and estimate volatility distributions for each asset.

The following cryptocurrencies were included in the analysis:
Bitcoin
Ethereum
Cardano
Solana
Chainlink

Methodology-
-Historical price data was downloaded using the yfinance library.
-The log returns were calculated using which measured the daily percentage change in prices.
-Volatility was estimated using a Bayesian model, assuming returns follow a normal distribution with volatility parameter.The posterior distribution of volatility was   sampled using a Metropolis-Hastings MCMC algorithm.
-An equal-weight portfolio was constructed where each cryptocurrency has weight 0.2.
-Portfolio volatility was calculated using the covariance matrix of returns.

Results-
-Posterior volatility distributions were estimated for each cryptocurrency
-Mean volatility and 95% credible intervals were computed.
-A comparison of individual coin risk and portfolio risk was visualized using bar plot.

Tools and Libraries-
Python
Numpy
Pandas
Matplotlib
yfinance

Conclusion-The equal-weight portfolio demonstrates diversification benefits, as the combined portfolio risk is more stable compared to the most volatile individual assets.
