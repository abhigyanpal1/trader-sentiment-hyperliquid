## 📊 Results & Insights

The analysis revealed clear relationships between **market sentiment** and **trader performance**:

### 1. Performance by Sentiment
- Traders, on average, showed **higher daily PnL during “Greed” periods** compared to “Fear”.
- This effect was consistent across most accounts, suggesting sentiment-driven market conditions influence profitability.

### 2. Sentiment Transitions Matter
- When the sentiment **shifted from Fear → Greed**, next-day PnL tended to improve.
- Conversely, **Greed → Fear** transitions were often followed by lower next-day returns.
- This indicates potential for **transition-based trading strategies**.

### 3. Key Drivers (Feature Importance from LightGBM)
The most influential factors for predicting daily PnL included:
1. **Trade Notional Value** (size × price)
2. **Recent PnL Trend** (last 3–5 days)
3. **Leverage Used**
4. **Market Sentiment Classification**

### 4. Strategy Implications
- Incorporating **Fear/Greed index** data alongside trader-specific metrics could help **optimize position sizing** and **risk management**.
- Transition-aware approaches may add an **edge** over using raw sentiment alone.

---

## 📂 Example Outputs
- **Figures**
  - `avg_pnl_by_sentiment.png` → Average daily PnL per sentiment type.
  - `nextday_pnl_by_transition.png` → Next-day returns by sentiment transition.
  - `feature_importances.png` → LightGBM feature importance chart.

- **Tables**
  - `account_day_panel.csv` → Cleaned & aggregated per-account, per-day metrics.
  - `feature_importances.csv` → Ranked list of predictive features.
  - `quick_summary.json` → Machine-readable summary of results.

---
