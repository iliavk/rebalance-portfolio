# Rebalancing a 2-Asset Portfolio: T-Bills and S&P 500

This project simulates and analyzes a simple portfolio rebalancing strategy involving two asset classes:
- 🧾 **T-Bills** (risk-free asset)
- 📈 **S&P 500 Index** (risky asset)

We aim to maintain a constant 30% / 70% allocation between T-Bills and the S&P 500, and compare portfolio performance under different rebalancing strategies.

---

## 🚀 Project Goals

- Implement a basic 2-asset portfolio with a 70/30 S&P/T-Bill allocation
- Simulate portfolio evolution with:
  - No rebalancing (buy and hold)
  - Time-based rebalancing (monthly, quarterly)
  - Threshold-based rebalancing
- Analyze key performance metrics: returns, volatility, drawdowns, Sharpe ratio
- Visualize portfolio behavior over time

---

## 📊 Technologies

- Python
- Pandas, NumPy, Matplotlib, Seaborn
- yfinance (for historical data)
- (Optional) pandas-datareader / FRED API

---

## 📁 Project Structure

```
rebalance-portfolio/
├── notebooks/
│   └── rebalance_simulation.ipynb     # Main analysis notebook
├── data/                              # Data storage (optional)
├── requirements.txt                   # List of Python dependencies
├── README.md                          # This file
```

---

## 📈 Sample Outputs (Coming Soon)

- Cumulative portfolio value comparison
- Asset weight drift over time
- Risk-return summary table

---

## 💡 Future Extensions

- Add transaction costs and taxes
- Dynamic (volatility-sensitive) rebalancing
- Add more asset classes (e.g., crypto)
- Reinforcement learning rebalancer (if you're feeling spicy 🌶️)

---

## 👨‍💻 Author

Ilia Krillov  
Math PhD pivoting into finance and quantitative research.  
📍 Based in Canada / Netherlands  
🚀 Open to data science, quant, and trading-related roles

---

## 📬 Contact

- [LinkedIn](https://www.linkedin.com/)ilia-v-kirillov
- Email: ilia.v.kirillov@gmail.com
