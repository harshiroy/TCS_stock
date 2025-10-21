# 📊 TCS Stock Data Analysis and Prediction

## 📘 Overview
This project analyzes **Tata Consultancy Services (TCS)** stock data to uncover historical trends and predict future prices using both **Linear Regression** and **LSTM Neural Networks**.

It merges three CSV datasets:

- `TCS_stock_history.csv` – OHLC + Volume  
- `TCS_stock_action.csv` – Dividends & Stock Splits  
- `TCS_stock_info.csv` – Additional Stock Details  

---

## 🎯 Objectives
- 📂 Combine historical, dividend, and split data  
- 📊 Explore trends using rich visualizations  
- 🤖 Build predictive models for closing prices  
- ⚖️ Compare regression vs. deep learning performance  

---

## 🧰 Tools & Libraries

| Purpose | Library |
|----------|----------|
| **Data Handling** | `pandas`, `numpy` |
| **Visualization** | `matplotlib`, `seaborn` |
| **Machine Learning** | `scikit-learn` |
| **Deep Learning** | `tensorflow` (LSTM) |
| **Progress Tracking** | `tqdm` |

---

## 📈 Analysis Workflow

### 1️⃣ Exploratory Data Analysis (EDA)
- Price trends and volume visualization  
- Moving averages (SMA, EMA)  
- Correlation heatmaps  

### 2️⃣ Feature Engineering
- Lag variables (previous day close, etc.)  
- Date-based splits for training and testing  

### 3️⃣ Modeling
- **Linear Regression** – baseline model  
- **LSTM (Long Short-Term Memory)** – sequence-based model  

### 4️⃣ Evaluation Metrics
- 📉 **MSE** (Mean Squared Error)  
- 📈 **R² Score** (Goodness of Fit)  
- ⚙️ **MAE** (Mean Absolute Error)

---

## 🔍 Key Insights
- 📊 `Close`, `High`, and `Low` prices are **highly correlated (r > 0.99)**  
- 💸 `Volume` and `Dividends` have minimal effect on short-term price changes  
- 🧠 LSTM model effectively tracks stock movement with **~₹70 average prediction error**

---

## 📦 requirements.txt
```txt
pandas
numpy
matplotlib
seaborn
scikit-learn
tensorflow
tqdm

🧠 Future Enhancements

🔮 Try ARIMA or Prophet for time-series forecasting

📊 Build an interactive dashboard using Plotly Dash

⚡ Automate data updates via Yahoo Finance API

📂 TCS_Stock_Analysis/
├── TCS_stock_history.csv
├── TCS_stock_action.csv
├── TCS_stock_info.csv
├── TCS_pipeline.ipynb
├── requirements.txt
└── README.md
🏁 Results Preview

📉 Linear Regression: Simple trend following

🤖 LSTM: Captures temporal patterns and volatility

📈 Visualized prediction vs. actual price chart
