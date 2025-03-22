# amd-nvda-stock-analysis
A comparative stock analysis of AMD and NVIDIA (2018–2025)
# 📊 Comparative Stock Analysis: NVIDIA vs AMD (2018–2025)

This project presents a comprehensive data-driven analysis of two major semiconductor companies: **NVIDIA (NVDA)** and **AMD**. The study uses Python, yFinance API, and Plotly to explore trends in stock prices, technical indicators, financial metrics, and predictive modeling.

## 🔍 Objectives

- Compare stock performance and volatility from 2018 to early 2025
- Visualize and interpret technical trends using MA indicators
- Analyze valuation metrics (P/E, EPS, Market Cap)
- Build a regression model to forecast next-day prices
- Test a simple MA crossover trading strategy (with and without U.S. SEC tax)
- Compare performance to a buy-and-hold strategy

## 🧰 Tools Used

- Python (Pandas, NumPy, yFinance, Scikit-learn)
- Plotly for interactive visualizations
- Matplotlib
- Jupyter Notebook

## 🗂️ Project Structure

```
📁 amd-nvda-stock-analysis/
├── AMDvsNVIDIA.ipynb       # Main notebook
├── README.md               # Project overview
└── requirements.txt        # Package dependencies
```

## 📈 Key Sections in the Notebook

1. **Data Collection**  
   Adjusted daily closing prices from Yahoo Finance (2018–2025)

2. **Return & Volatility Analysis**  
   Daily returns and annualized volatility show NVIDIA is higher risk/higher reward

3. **Technical Indicators**  
   MA20 and MA50 crossovers analyzed with visualizations

4. **Fundamental Comparison**  
   NVIDIA leads in P/E, EPS, and Market Cap

5. **Machine Learning Forecasting**  
   Linear Regression used to predict next-day prices with past 5-day windows

6. **Trading Strategy Backtest**  
   MA20/MA50 crossover strategy tested for both tickers, with and without SEC tax

7. **Buy-and-Hold Comparison**  
   Strategy performance is benchmarked against simple buy-and-hold

---

## 💹 Strategy Evaluation Summary

We implemented a moving average crossover strategy using MA20 and MA50. The strategy generated 19 trades for both AMD and NVIDIA over the 2018–2025 period.

| Stock | Total Return (No Tax) | Total Return (With Tax) | Trades | Avg Trade Return |
|-------|------------------------|--------------------------|--------|------------------|
| AMD   | 283.98%                | 283.93%                  | 19     | 10.42%           |
| NVDA  | 746.82%                | 746.69%                  | 19     | 16.45%           |

- **NVIDIA significantly outperformed AMD**, consistent with its AI-driven growth trend.
- **SEC tax impact is negligible** due to its low rate (0.0008%), but real-world brokerage fees and slippage are not included.
- Strategy shows promise in trending markets but may underperform in strong bull runs.

---

## 📉 Buy-and-Hold vs Strategy Results

We compared the cumulative return of the MA strategy to a simple buy-and-hold strategy.

- For both stocks, **buy-and-hold outperformed** the MA strategy over this time period.
- This is likely because the market trend was strongly bullish, favoring long-term holding over frequent switching.

---

## 📬 Contact

Feel free to connect if you'd like to discuss this project or data science in finance!

---

## 🧠 Strategy Reflection & Limitations

### 📌 Personal Acknowledgement
As a student still learning investment analysis and financial modeling, my understanding of real-world strategy design is evolving. This project represents my best effort to apply classroom knowledge to practical data-driven trading ideas.

### ⚠️ Strategy Limitations
- **Execution Assumptions**: The strategy assumes perfect trade execution without slippage, bid-ask spread, or liquidity constraints.
- **No Capital Allocation**: It doesn't account for position sizing or portfolio diversification.
- **No Walk-Forward Validation**: There's no out-of-sample testing or cross-validation for robustness.
- **Static Parameters**: MA periods are fixed and not optimized per asset or volatility regime.
- **Simple ML**: The forecasting model only uses past prices; it lacks external features like volume, macro data, or market sentiment.

---

### 🎯 Future Learning Goals

- Learn advanced backtesting frameworks (e.g., `backtrader`, `quantconnect`)
- Study risk-adjusted evaluation metrics and portfolio theory
- Explore dynamic and adaptive trading systems
- Integrate macroeconomic indicators and market structure features
- Implement more sophisticated machine learning models (LSTM, tree-based models)

This project is a foundation I aim to build upon as I grow into the data science and quantitative finance field.
