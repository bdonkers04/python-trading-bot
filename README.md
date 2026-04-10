# 📈 Crypto Trading Bot (RSI + SMA Strategy)

> A Python-based backtesting script that uses technical indicators (RSI, SMA, momentum, MACD, OBV) to simulate a crypto trading strategy on historical Binance data.

---

## 🚀 Overview

This project fetches **1-minute candlestick data (30 days)** from Binance and applies a rule-based trading strategy:

- 📉 **Buy** when the asset is oversold (low RSI) and below the moving average  
- 📈 **Sell** when profit target is hit or price weakens  
- 💰 Tracks portfolio growth over time  

It also exports indicator data to CSV for further analysis.

---

## 🧠 Strategy Logic

### Buy Condition
- RSI < 20 (oversold)
- Price < 20-period SMA

### Sell Conditions

**Take Profit**
- Price > SMA  
- Gain > 0.1%  

**Stop Loss**
- Price drops below buy price  

---

## 🛠️ Tech Stack

- Python
- NumPy
- TA-Lib
- Binance API
- Matplotlib
- CSV

---

## 📦 Installation

### 1. Clone the repo
```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
