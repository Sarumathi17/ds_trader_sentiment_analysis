# 📊 Trader Performance vs Market Sentiment Analysis

## 🧩 Project Overview
This project explores how **market sentiment** — categorized as *Fear*, *Greed*, *Extreme Fear*, *Extreme Greed*, and *Neutral* — impacts **trader performance** and **trading behavior**.  
By analyzing profit/loss (`ClosedPnL`), trade sizes, and trading sides (BUY/SELL), this project uncovers behavioral patterns that reveal how emotions influence market activity.

---

## 🎯 Objective
> To explore the relationship between trader performance and market sentiment, uncover hidden patterns, and deliver insights that can drive smarter trading strategies.

---

## 📂 Folder Structure
```text
📁 ds_trader_sentiment_analysis/
│
├── csv_files/
|   ├── historical_data.csv 
│   ├── fear_greed_index.csv
│   ├── merged_trades_with_sentiment.csv
│   └── cleaned_trading_data.csv
│
├── outputs/
│   ├── avg_pnl_by_sentiment.png
│   ├── correlation_heatmap.png
│   ├── pairplot_multivariate.png
│   ├── pnl_distribution.png
│   ├── sentiment_distribution.png
│   ├── side_distribution.png
│   ├── trade_size_by_sentiment.png
│   └── trade_size_usd_distribution.png
│
├── notebook_1.ipynb
├── ds_report.pdf
└── README.md
```

> ⚠️ Due to GitHub’s file size limitations, the following large CSV files are **not uploaded** to this repository.  
> You can download them using the link below:

| File Name | Description | Download Link |
|------------|-------------|----------------|
| **historical_data.csv** | Raw trade-level data containing execution details, trade size, and profit/loss information. | [📥 Download historical_data.csv]([https://drive.google.com/your-shared-link-here](https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjV)) |
| **merged_trades_with_sentiment.csv** | Final merged dataset combining trade data with sentiment classifications. | *generate from notebook* |
---

## ⚙️ Setup Instructions

### 🧠 Requirements
- Python 3.x  
- Required Libraries:  
  ```bash
  pip install pandas numpy matplotlib seaborn

### ▶️ Running the Notebook

1. Open the `notebook_1.ipynb` file in **Google Colab** or **Jupyter Notebook**.  
2. Upload the data files:
   - `historical_data.csv`
   - `fear_greed_index.csv`
   into the `/csv_files` folder.  
3. Run the notebook cells sequentially in this order:
   - **Data Loading**
   - **Data Cleaning** (handle missing values)
   - **Exploratory Data Analysis (EDA)**
4. View generated visualizations inside the `/outputs` folder.

---

## 📊 Key Insights Summary

| Topic | Observation |
|-------|--------------|
| **Trader Behavior** | Most trades occur during *Fear* and *Greed* phases — emotional markets drive participation. |
| **Profitability** | *Extreme Greed* yields highest average profits, while *Extreme Fear* shows lowest returns. |
| **Trade Size** | Majority of trades are small, reflecting cautious trading; few large trades indicate institutional activity. |
| **Sentiment Impact** | Trader performance improves with market optimism but also shows higher volatility. |
| **Correlations** | Weak correlation between `closed_pnl` and numeric variables → profitability is sentiment-driven, not numeric. |

---

## 🧠 Insights Summary

- **Trader performance peaks in Greed phases** when confidence is high.  
- **Fear phases** show smaller trades and lower profit, reflecting defensive trading.  
- **Extreme Greed** brings high potential profits but increased risk and variability.  
- **Market sentiment strongly drives trading volume, exposure, and performance.**

---

## 💡 Recommendations

- Develop **sentiment-aware trading systems** that adjust strategies dynamically based on Fear-Greed indices.  
- Implement **risk controls during Extreme Fear** phases to prevent panic selling.  
- Use **position-size caps** during Greed phases to mitigate overexposure.  
- Combine historical trade data with sentiment signals to improve forecasting models.

---

## 🧮 Tools & Technologies

- **Python**  
- **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**  
- **Jupyter Notebook / Google Colab**

---

## 📈 Output Examples

| Visualization | Description |
|----------------|-------------|
| 📊 *Market Sentiment Distribution* | Shows how trades are distributed across Fear/Greed phases. |
| 📈 *Average ClosedPnL by Sentiment* | Highlights how trader profitability changes with market emotion. |
| 📦 *Trade Size Distribution* | Displays skewness and concentration of trade volumes. |
| 🔥 *Correlation Heatmap* | Shows interdependence of numeric features. |
| 🎨 *Pair Plot* | Visualizes multivariate sentiment-based relationships. |

---

## 🧾 Author

**👩‍💻 Sarumathi M**  
Data Science Enthusiast  
📧 *msarumathi2@gmail.com*  
📅 *November 2025*

---

## ✅ Conclusion

This project reveals that trader behavior and profitability are **deeply linked to market sentiment**.  
Periods of Greed correlate with higher profits and volatility, while Fear phases lead to lower activity and smaller trades.  
Understanding these emotional dynamics can enhance **trading strategy design**, **risk management**, and **market timing decisions**.
