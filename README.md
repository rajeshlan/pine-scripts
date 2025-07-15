# 📦 Probable Order Blocks Indicators Collection

This repository contains a suite of **Pine Script v6** indicators built for **Smart Money Concept (SMC)** and **price action traders**. These tools help detect and visualize **Order Blocks (OBs)**—key institutional price zones—along with optional alerts and signal generation.

---

## 📂 Included Scripts

| File Name                                         | Description                               | Alerts | Buy/Sell Signals | Auto Cleanup | Use Case                    |
| ------------------------------------------------- | ----------------------------------------- | ------ | ---------------- | ------------ | --------------------------- |
| `order_blocks_reversal_continuation_v1.pine`      | Basic OB detection and visualization      | ❌      | ❌                | ❌            | Learning OB structure       |
| `order_blocks_reversal_continuation_alerts.pine`  | Adds alerts when price re-enters OB zones | ✅      | ❌                | ❌            | Passive zone watching       |
| `order_blocks_signals.pine`                       | Adds signal confirmation inside OB zones  | ✅      | ✅                | ✅            | Signal-based OB trading     |
| `order_blocks_reversal_continuation_compact.pine` | Minimalist version with OB plotting only  | ❌      | ❌                | ❌            | Lightweight overlay use     |
| `order_blocks_clean_signal.pine`                  | Complete system: OBs + signals + cleanup  | ✅      | ✅                | ✅            | Practical, clean OB trading |

---

## 📘 Script Details

### 1. `order_blocks_reversal_continuation_v1.pine`

* Detects swing highs/lows and BOS (Break of Structure)
* Marks the last opposite candle before BOS as an Order Block
* Plots OB zones using green (bullish) and red (bearish) boxes
* Adds optional labels: "Reversal" or "Continuation"

**Best For:** Beginners learning OB detection visually

---

### 2. `order_blocks_reversal_continuation_alerts.pine`

* All features from `v1`
* Adds alert conditions when price re-enters OB zones

**Best For:** Traders who want to monitor OB reactions without watching charts constantly

---

### 3. `order_blocks_signals.pine`

* Adds candle confirmation logic inside OB zones
* Plots BUY/SELL signal labels based on bullish/bearish closes
* Includes alerts for signals
* Auto-cleans expired OB boxes after a set number of bars

**Best For:** Active traders looking for semi-automated OB signal generation

---

### 4. `order_blocks_reversal_continuation_compact.pine`

* Slimmed-down version
* Draws OB boxes only (no alerts, no logic overhead)

**Best For:** Traders wanting fast, clean OB plots without signal distractions

---

### 5. `order_blocks_clean_signal.pine`

* Most complete and production-ready version
* Combines:

  * BOS detection
  * OB zone drawing
  * Signal confirmation
  * Auto-cleanup of old boxes
  * Real-time alerts

**Best For:** Practical OB-based trading setups with low noise and high clarity

---

## 📌 Notes

* All scripts are written in **Pine Script v6**
* Designed for use on any market: crypto, forex, stocks
* Customize `structure_lookback` and `impulse_candles` to fit your strategy or time frame

---

## 🚀 Contributing

Pull requests are welcome. If you'd like to improve logic, visuals, or performance, feel free to fork and propose changes.

## 📧 Contact

Have questions or ideas? Open an issue or message directly via GitHub.

---

Happy Trading 📈
