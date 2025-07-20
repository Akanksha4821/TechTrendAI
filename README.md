# TechTrendAI

# 📈 Trading Strategies Analysis

This project implements and analyzes multiple trading strategies using Python and historical financial data. It provides signal generation and return analysis for:

- ✅ Relative Strength Index (RSI)
- ✅ Moving Average Convergence Divergence (MACD)
- ✅ Bollinger Bands (BB)
- ✅ A Mixed Strategy (combining MACD and BB)

## 📊 Strategies Overview

---

### 1. **Relative Strength Index (RSI)**

**Calculation:**
- Compute daily gains and losses over a 14-day period.
- Calculate Average Gain and Average Loss.
- Derive RSI using the formula:  
  `RSI = 100 - (100 / (1 + RS))` where RS = AG / AL

**Signals:**
- 📉 Buy when RSI < 30 (oversold)
- 📈 Sell when RSI > 70 (overbought)

**Returns:**
- Calculated based on signal-driven entry and exit points.

---

### 2. **Moving Average Convergence Divergence (MACD)**

**Calculation:**
- Compute 12-day and 26-day Exponential Moving Averages (EMAs)
- MACD = EMA(12) - EMA(26)
- Signal Line = EMA(9) of MACD
- Histogram = MACD - Signal Line

**Signals:**
- 📉 Buy when MACD crosses above Signal Line
- 📈 Sell when MACD crosses below Signal Line

**Returns:**
- Evaluated using crossover-based trades.

---

### 3. **Bollinger Bands (BB)**

**Calculation:**
- 14-day Simple Moving Average (SMA)
- 14-day rolling Standard Deviation
- Upper Band = SMA + 2 * STD
- Lower Band = SMA - 2 * STD

**Signals:**
- 📉 Buy when price dips below Lower Band
- 📈 Sell when price crosses above Upper Band

**Returns:**
- Based on price reversion trades.

---

### 4. **Mixed Strategy**

**Signals:**
- 📉 Buy when MACD is above Signal Line **and** price is near or below the lower Bollinger Band.
- 📈 Sell when price exceeds the upper Bollinger Band.

**Returns:**
- Combines strengths of both indicators for more refined entries/exits.

---


