# 📊 Finance & Risk Analytics Dashboard

> **A production-grade quantitative finance project** covering portfolio analysis, risk metrics, ML-powered price prediction, and Monte Carlo simulation — built end-to-end in Python.

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?style=flat&logo=pandas)
![Plotly](https://img.shields.io/badge/Plotly-Interactive-3F4F75?style=flat&logo=plotly)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E?style=flat&logo=scikit-learn)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter)

---

## 🗂️ Project Overview

This project simulates a **real-world quantitative analyst workflow** — from data ingestion through risk reporting and predictive modelling — applied to an 8-stock tech/finance portfolio.

| Area | What's Covered |
|------|---------------|
| **Portfolio Analysis** | Cumulative returns, annual alpha vs SPY benchmark, allocation |
| **Risk Metrics** | Historical VaR, Parametric VaR, CVaR, Sharpe, Sortino, Beta, Max Drawdown, Calmar |
| **Correlation Analysis** | Pairwise heatmap, rolling 60-day correlation vs benchmark |
| **ML Prediction** | Random Forest + Gradient Boosting with 25+ technical features, TimeSeriesSplit CV |
| **Monte Carlo** | 10,000 correlated asset paths via Cholesky decomposition |
| **Dashboard** | 9-panel interactive Plotly dashboard with hover, zoom & filter |

---

## 🚀 Quickstart

```bash
# 1. Clone the repository
git clone https://github.com/madhura-23/100-days-code.git
cd "100-days-code/Finance_Risk_Analytics"

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch the notebook
jupyter notebook Finance_Risk_Analytics.ipynb
```

---

## 📦 Dependencies

```txt
yfinance>=0.2.36
pandas>=2.0
numpy>=1.26
scipy>=1.11
scikit-learn>=1.3
plotly>=5.18
matplotlib>=3.8
seaborn>=0.13
jupyter>=1.0
ipywidgets>=8.0
```

---

## 🔬 Methodology

### Risk Metrics

| Metric | Formula / Method |
|--------|-----------------|
| **Historical VaR (95%)** | 5th percentile of empirical return distribution |
| **Parametric VaR (95%)** | μ + z₀.₀₅ × σ (Normal assumption) |
| **CVaR / Expected Shortfall** | Mean of returns below VaR threshold |
| **Sharpe Ratio** | `(R_p - R_f) / σ_p × √252` |
| **Sortino Ratio** | `(R_p - R_f) / σ_downside × √252` |
| **Beta** | `Cov(R_p, R_m) / Var(R_m)` |
| **Max Drawdown** | `min((P_t - max(P_0..P_t)) / max(P_0..P_t))` |
| **Calmar Ratio** | `Ann. Return / |Max Drawdown|` |

### ML Feature Engineering (25+ features)

- **Lag returns**: 1, 2, 3, 5, 10, 21 days
- **Rolling statistics**: mean, std, skewness, kurtosis (5/10/21/63-day)
- **Momentum**: price ratio over 5, 21, 63, 126-day windows
- **Volatility regime**: realised vol, vol ratio
- **Technical indicators**: RSI-14, MACD, MACD signal, Bollinger Band position
- **Target**: 5-day forward log-return (no data leakage)

### Monte Carlo

Uses **Cholesky decomposition** of the historical covariance matrix to simulate 10,000 correlated multi-asset paths over 252 trading days, preserving realistic cross-asset dependencies.

---

## 📈 Sample Outputs

```
Portfolio Metrics (Example — actual values depend on run date)
─────────────────────────────────────────────────────────────
Annualised Return        ~28%
Annualised Volatility    ~22%
Sharpe Ratio             ~1.18
Sortino Ratio            ~1.65
Historical VaR (95%)     ~1.9%/day
Max Drawdown             ~-35%
─────────────────────────────────────────────────────────────
ML Directional Accuracy  ~56–58%  (>55% = useful in quant finance)
─────────────────────────────────────────────────────────────
Monte Carlo (10k paths)
  Expected Final Value    > initial capital
  P(Loss after 1 year)    < 20%
─────────────────────────────────────────────────────────────
```

---

## 🗃️ Repository Structure

```
Finance_Risk_Analytics/
├── Finance_Risk_Analytics.ipynb   ← Main notebook (all analysis)
├── README.md
└── requirements.txt
```

---

## 🔭 Extensions / Future Work

- [ ] **Efficient Frontier** — Mean-variance portfolio optimisation
- [ ] **Factor Model** — Fama-French 3/5-factor decomposition
- [ ] **Options Pricing** — Black-Scholes, implied vol surface
- [ ] **LSTM Model** — Sequence-based deep learning prediction
- [ ] **Streamlit App** — Deploy as a live web dashboard
- [ ] **Real-Time Alerts** — VaR breach / drawdown notifications

---

## 🤝 Author

**Madhura** · [GitHub](https://github.com/madhura-23)

---

## 📝 License

MIT — free to fork, adapt, and build upon.
