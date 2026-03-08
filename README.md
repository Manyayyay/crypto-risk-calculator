# crypto-risk-calculator
crypto-risk-calculator using MCMC
This project analyzes the volatility (risk) of cryptocurrencies using Bayesian MCMC. The goal is to estimate the volatility of individual assets and evaluate the risk of an equal-weight cryptocurrency portfolio.The analysis uses historical price data to compute log returns and estimate volatility distributions for each asset.

The following cryptocurrencies were included in the analysis:<br>
Bitcoin<br>
Ethereum<br>
Cardano<br>
Solana<br>
Chainlink<br>

Methodology-<br>
-Historical price data was downloaded using the yfinance library.<br>
-The log returns were calculated using which measured the daily percentage change in prices.<br>
-Volatility was estimated using a Bayesian model, assuming returns follow a normal distribution with volatility parameter.The posterior distribution of volatility was   sampled using a Metropolis-Hastings MCMC algorithm.<br>
-An equal-weight portfolio was constructed where each cryptocurrency has weight 0.2.<br>
-Portfolio volatility was calculated using the covariance matrix of returns.<br>

Results-<br>
-Posterior volatility distributions were estimated for each cryptocurrency<br>
-Mean volatility and 95% credible intervals were computed.<br>
-A comparison of individual coin risk and portfolio risk was visualized using bar plot.<br>

Tools and Libraries-<br>
Python<br>
Numpy<br>
Pandas<br>
Matplotlib<br>
yfinance<br>

Conclusion-The equal-weight portfolio demonstrates diversification benefits, as the combined portfolio risk is more stable compared to the most volatile individual assets.
