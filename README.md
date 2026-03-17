# 🖥️ Python GUI Projects

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Tkinter](https://img.shields.io/badge/Tkinter-GUI-FF6B35?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-JSX-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)

**A growing collection of GUI applications, games, and dashboards built with Python & JavaScript.**

</div>

---

## 📂 Projects

### 1. 🧮 Finance & Risk Analytics Dashboard
> **Type:** Data Analytics · Machine Learning · Interactive Dashboard

A production-grade quantitative finance engine built entirely in Python. Covers portfolio analysis vs S&P 500, full risk metrics suite, ML-based price prediction, and Monte Carlo simulation.

| Feature | Details |
|---------|---------|
| Portfolio Analysis | Cumulative returns, annual alpha vs SPY benchmark |
| Risk Metrics | VaR, CVaR, Sharpe, Sortino, Beta, Max Drawdown, Calmar |
| ML Prediction | Random Forest + Gradient Boosting with 25+ technical features |
| Monte Carlo | 10,000 correlated paths via Cholesky decomposition |
| Dashboard | 9-panel interactive Plotly dashboard |

**Tech:** `Python` `Pandas` `NumPy` `Scikit-learn` `Plotly` `yfinance`

📁 [`Finance-Risk-Analytics/`](./Finance-Risk-Analytics)

---

### 2. ✅ Habit Tracker GUI
> **Type:** Desktop GUI Application · Data Visualisation

A desktop habit tracking application built with **Tkinter** featuring daily habit logging, statistics tracking, and a heatmap visualisation showing consistency over time — similar to GitHub's contribution graph.

| Feature | Details |
|---------|---------|
| Habit Logging | Add, complete, and delete daily habits |
| Statistics | Streaks, completion rates, and weekly summaries |
| Heatmap | Visual calendar heatmap of habit consistency |
| Persistence | Data saved locally across sessions |

**Tech:** `Python` `Tkinter` `Matplotlib` `JSON`

📁 [`HabitTrackerGUI`](./HabitTrackerGUI)

---

### 3. ❌⭕ Tic Tac Toe 1.0
> **Type:** Desktop GUI Game · Python Tkinter

An interactive **Tic Tac Toe** game with a full graphical interface built using Tkinter. Two-player mode with win detection, draw detection, and a reset button.

| Feature | Details |
|---------|---------|
| 2-Player Mode | Take turns as X and O |
| Win Detection | Checks all rows, columns, and diagonals |
| Draw Detection | Handles board-full stalemate |
| Reset | One-click game restart |

**Tech:** `Python` `Tkinter`

📁 [`Tic-Tak-Toe 1.0/`](./Tic-Tak-Toe%201.0)

---

### 4. 📊 Life Dashboard
> **Type:** React Component · Personal Productivity

A React-based personal life dashboard (`Lifedashboard.jsx`) for tracking goals, tasks, and daily productivity metrics in a single interactive view.

**Tech:** `React` `JSX` `JavaScript` `CSS`

📄 [`Lifedashboard.jsx`](./Lifedashboard.jsx)

---

### 5. 💡 LeetCode Solutions
> **Type:** Problem Solving · Algorithms & Data Structures

A collection of LeetCode problem solutions written in Python, covering arrays, strings, dynamic programming, and more.

**Tech:** `Python`

📄 [`Leetcode Solution`](./Leetcode%20Solution)

---

## 🚀 Getting Started

### Run Python GUI Projects

```bash
# Clone the repository
git clone https://github.com/madhura-23/python-gui-projects.git
cd python-gui-projects

# Install dependencies
pip install matplotlib pandas numpy plotly yfinance

# Run Habit Tracker
python HabitTrackerGUI

# Run Tic Tac Toe
cd "Tic-Tak-Toe 1.0"
python main.py
```

### Run Finance & Risk Analytics

```bash
cd Finance-Risk-Analytics
pip install -r requirements.txt
python -m jupyter lab Finance_Risk_Analytics.ipynb
```

---

## 🛠️ Tech Stack

| Language / Library | Used In |
|-------------------|---------|
| Python 3.10+ | All Python projects |
| Tkinter | Habit Tracker, Tic Tac Toe |
| Matplotlib / Seaborn | Habit Tracker heatmap, Finance charts |
| Pandas / NumPy | Finance & Risk Analytics |
| Plotly | Finance interactive dashboard |
| Scikit-learn | ML price prediction |
| yfinance | Live stock data |
| React / JSX | Life Dashboard |
| JavaScript | Game logic |

---

## 📁 Repository Structure

```
python-gui-projects/
│
├── Finance-Risk-Analytics/     ← Quant finance notebook & dashboard
├── Tic-Tak-Toe 1.0/            ← Tkinter GUI game
├── HabitTrackerGUI             ← Tkinter habit tracking app
├── Lifedashboard.jsx           ← React personal dashboard
├── Leetcode Solution           ← Python algorithm solutions
├── random_1.py                 ← Python practice scripts
└── README.md
```

---

## 🔭 Upcoming Projects

```
[ ] Weather App          — Live weather with OpenWeatherMap API
[ ] Expense Tracker      — GUI with charts and CSV export
[ ] Pomodoro Timer       — Productivity timer with Tkinter
[ ] Password Manager     — Encrypted local password vault
[ ] Snake Game           — Classic game with Tkinter canvas
```

---

## 👩‍💻 Author

**Madhura**
GitHub: [@madhura-23](https://github.com/madhura-23)
Domain: Data Analytics · Python Development · GUI Applications

---

<div align="center">

*If you find any project useful, consider giving the repo a ⭐ — it helps a lot!*

</div>
