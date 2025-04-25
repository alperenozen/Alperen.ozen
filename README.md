# 📈 Analyzing the Influence of Bitcoin (BTC) and Solana (SOL) Price Movements on Meme Coin Market Capitalization

## 📌 Project Overview
This project investigates the relationship between the price movements of **Bitcoin (BTC)** and **Solana (SOL)** and the market capitalization of two leading meme coins: **Dogecoin (DOGE)** and **Shiba Inu (SHIB)**.  
The goal is to determine whether fluctuations in BTC and SOL prices significantly affect meme coin market behavior.

## 🎯 Motivation
Meme coins are highly speculative assets that often follow broader market sentiment. By understanding whether major cryptocurrencies like Bitcoin and Solana influence meme coins, we can uncover valuable insights for investors, traders, and researchers interested in crypto market dynamics.

---

## 📊 Hypotheses

### 1. Bitcoin (BTC) Price Influence
- **Null Hypothesis (H₀):** Bitcoin price movements do not significantly affect meme coin market capitalization.
- **Alternative Hypothesis (Hₐ):** Bitcoin price movements significantly and positively influence meme coin market capitalization.

### 2. Solana (SOL) Price Influence
- **Null Hypothesis (H₀):** Solana price movements do not significantly affect meme coin market capitalization.
- **Alternative Hypothesis (Hₐ):** Solana price movements significantly and positively influence meme coin market capitalization.

### 3. Combined BTC & SOL Influence
- **Null Hypothesis (H₀):** BTC and SOL price movements together do not significantly influence meme coin market capitalization.
- **Alternative Hypothesis (Hₐ):** BTC and SOL price movements together significantly influence meme coin market capitalization.

---

## 📥 Data Collection

### ⚠️ Note on Data Sources
Originally planned sources from Kaggle and CoinMarketCap were not used due to missing or inconsistent historical `.csv` data.  
Instead, all data was collected using the **`yfinance`** library for real-time reliability.

### ✅ Assets Used
- **BTC-USD** – Bitcoin price and returns
- **SOL-USD** – Solana price and returns
- **DOGE-USD** – Dogecoin market cap (derived)
- **SHIB-USD** – Shiba Inu market cap (derived)
- **PEPE-USD** – **Excluded** due to insufficient historical range (~4 months)

### 🕒 Time Range
- Aligned daily data from **2020-08-01** to **2025-04-24**

---

## 🧹 Data Processing

- **Missing Values:** Forward-filled missing values to ensure alignment
- **Market Cap Calculation:**  
  \[
  \text{Market Cap} = \text{Close Price} \times \text{Circulating Supply}
  \]
- **Normalization:** Applied Min-Max scaling for visualization
- **PEPE Exclusion:** Removed due to limited historical range

---

## 📈 Statistical Analysis

### ✅ Techniques Used:
- Linear Regression (via `statsmodels`)
- Residual Diagnostics
- Pearson Correlation
- Rolling Correlation (30-day window)
- Data Normalization
- Scatter, Line, Histogram, and Heatmap Visualizations

---

## 📋 Results Summary

| Hypothesis | Variable Tested | Coefficient | p-value | R² | Conclusion |
|------------|------------------|-------------|---------|----|------------|
| **H1** | BTC Return → Meme Cap Return | `0.1124` | `0.000` | `0.131` | ✅ Significant |
| **H2** | SOL Return → Meme Cap Return | `0.0819` | `0.000` | `0.045` | ✅ Significant but weak |
| **H3** | BTC & SOL → Meme Cap Return | BTC: `0.1084`, SOL: `0.0091` | BTC: `0.000`, SOL: `0.378` | `0.132` | ✅ BTC significant, SOL not |

---

## 🧰 Tools and Technologies

- [Python](https://www.python.org/)
- [`yfinance`](https://pypi.org/project/yfinance/)
- `pandas`, `numpy` – Data preprocessing
- `matplotlib`, `seaborn` – Visualizations
- `statsmodels` – Regression analysis
- Google Colab / Jupyter Notebook

---

## 📌 Key Insights

- **Bitcoin Return is the dominant predictor** of meme coin market behavior.
- **Solana Return shows significance in isolation**, but not when BTC is included in the model.
- Investors may use **BTC trends as a leading indicator** for meme coin performance.

---

## 📆 Future Improvements

- Include **more meme coins** (e.g., FLOKI, PEPE) as longer datasets become available.
- Test **nonlinear models** or **Granger causality** to capture lagged effects.
- Incorporate **sentiment analysis** or **on-chain metrics** to improve prediction.

---

## 🧪 Conclusion

This project applied real market data and regression techniques to uncover the influence of BTC and SOL on meme coin markets.  
The findings confirm that **Bitcoin’s price movements have a statistically significant and positive influence**, while **Solana’s influence is marginal** when controlling for Bitcoin.

The analysis supports the idea that **BTC leads crypto market sentiment**, making it a valuable tool for anticipating meme coin behavior.

---
