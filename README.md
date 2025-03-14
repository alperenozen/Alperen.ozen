# Analyzing the Influence of Bitcoin (BTC) and Solana (SOL) Price Movements on Meme Coin Market Capitalization

## Project Overview
This project investigates the relationship between the price movements of Bitcoin (BTC) and Solana (SOL) and the market capitalization of the three popular meme coins: **Dogecoin (DOGE), Shiba Inu (SHIB),** and **Pepe Coin (PEPE)**. The goal is to understand if fluctuations in BTC and SOL prices significantly impact the market capitalization of these meme coins.

## Motivation
The cryptocurrency market is highly volatile, and meme coins often experience sudden market movements that may be influenced by major cryptocurrencies such as Bitcoin and Solana. Understanding the dynamics of how Bitcoin and Solana affect meme coin market caps can provide valuable insights for investors and traders in the crypto space.

## Hypotheses
1. **Bitcoin (BTC) Price Influence on Meme Coin Market Cap:**
   - **Null Hypothesis (H₀):** There is no significant relationship between Bitcoin's price movements and the market capitalization of meme coins.
   - **Alternative Hypothesis (Hₐ):** There is a significant positive correlation between Bitcoin's price movements and the market capitalization of meme coins. An increase in Bitcoin’s price will lead to an increase in meme coin market capitalization.

2. **Solana (SOL) Price Influence on Meme Coin Market Cap:**
   - **Null Hypothesis (H₀):** There is no significant relationship between Solana's price movements and the market capitalization of meme coins.
   - **Alternative Hypothesis (Hₐ):** There is a significant positive correlation between Solana's price movements and meme coin market capitalization.

3. **Combined Analysis of BTC and SOL Price Movements on Meme Coin Market Cap:**
   - **Null Hypothesis (H₀):** There is no significant relationship between the price movements of Bitcoin (BTC) and Solana (SOL) and the market capitalization of meme coins.
   - **Alternative Hypothesis (Hₐ):** Price movements of both Bitcoin and Solana significantly influence the market capitalization of meme coins.

## Data Collection
The data required for this project will be collected from the following sources:

1. **Bitcoin Price (BTC):**
   - Data on the daily closing price of Bitcoin will be sourced from [CoinMarketCap](https://www.coinmarketcap.com) or [CoinGecko](https://www.coingecko.com).

2. **Solana Price (SOL):**
   - Data on the daily closing price of Solana will be gathered from [CoinMarketCap](https://www.coinmarketcap.com) or [CoinGecko](https://www.coingecko.com).

3. **Meme Coin Market Capitalization:**
   - The daily market capitalization of the top three meme coins (DOGE, SHIB, PEPE) will be retrieved from [CoinMarketCap](https://www.coinmarketcap.com) or [CoinGecko](https://www.coingecko.com).

### Data Points to be Collected:
- **Bitcoin (BTC) Price:** Daily closing price (USD).
- **Solana (SOL) Price:** Daily closing price (USD).
- **Meme Coin Market Cap (DOGE, SHIB, PEPE):** Daily market capitalization (USD).
- **Date and Time:** Ensure all data is aligned by date for comparison.

## Data Processing and Analysis
1. **Data Preprocessing:**
   - Clean the data by handling missing values, ensuring consistency, and converting timestamps to a standard format.
   - Flag any outliers (such as data anomalies due to exchange issues or market crashes).
  
2. **Correlation Analysis:**
   - Use Pearson’s correlation coefficient to analyze the relationship between Bitcoin and Solana price movements and the market capitalization of the top three meme coins.
  
3. **Regression Analysis:**
   - Perform linear regression analysis to understand the strength and significance of the relationship between BTC/SOL price changes and meme coin market cap changes.
  
4. **Visualization:**
   - Scatter plots to show the relationship between Bitcoin/Solana price movements and meme coin market cap.
   - Line charts to observe the trends over time.
   - Heatmaps to show correlations.

## Expected Outcomes
1. **BTC Influence on Meme Coin Market Cap:**
   - We expect that when Bitcoin's price rises, meme coin market caps will likely increase as well, reflecting broader market sentiment.
  
2. **SOL Influence on Meme Coin Market Cap:**
   - Solana’s price movements may have a weaker correlation with meme coin market caps compared to Bitcoin, but still show some positive correlation in periods of market optimism.

3. **Combined Analysis:**
   - We expect Bitcoin’s price to have a more pronounced effect on meme coin market caps, but Solana’s price could provide additional insights during altcoin rallies.

## Tools and Technologies
- **Python** for data cleaning and statistical analysis.
- **Pandas** for data manipulation.
- **Matplotlib and Seaborn** for data visualization.
- **SciPy** for statistical testing (e.g., regression analysis).
- **Jupyter Notebooks** for interactive analysis and visualization.

## Plan for Data Collection
Data will be collected on a **daily basis** over a period of **3-6 months** to ensure a representative sample. The price data for Bitcoin, Solana, and the market caps of meme coins will be collected from CoinMarketCap and CoinGecko.

To ensure data accuracy, I will:
- Regularly update the dataset from the aforementioned sources.
- Flag and clean any anomalies or missing data points.
- Standardize the data format for consistency.

---

## Conclusion
This project aims to explore the relationship between the price movements of Bitcoin (BTC) and Solana (SOL) and the market capitalization of meme coins (DOGE, SHIB, and PEPE). By testing the outlined hypotheses, we hope to uncover patterns that can provide valuable insights for investors and help in predicting meme coin market behavior.

The final analysis will include visualizations, statistical tests, and actionable insights for traders and enthusiasts in the meme coin market.
