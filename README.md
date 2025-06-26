# Fear-Greed-Trading
# 🧠 Trader Behavior Insights Based on Bitcoin Market Sentiment

This data science project explores how **market sentiment** (Fear vs Greed) influences **trader behavior and performance** using historical trading data and sentiment index values.

## 📁 Datasets Used

1. **Bitcoin Market Sentiment Dataset**
   - Columns: `Date`, `Classification` (Fear/Greed), `Value` (0–100 scale)
   - Source: [Fear & Greed Index CSV](https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view)

2. **Hyperliquid Historical Trader Data**
   - Columns: `account`, `symbol`, `execution price`, `size`, `side`, `time`, `start position`, `event`, `closed pnl`, `size usd`, etc.
   - Source: [Trader History CSV](https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view)

---

## 🎯 Objective

The main goal is to explore the **relationship between trader performance and market sentiment**, uncover hidden behavioral patterns, and deliver insights to improve crypto trading strategies.

---

## 🔎 Key Questions Answered

### 1️⃣ Do traders make more money during **Greed** or **Fear**?

- Calculated average `closed pnl` (Profit & Loss) and win-rates across different sentiment bands (Extreme Fear → Extreme Greed).
- Visualized % of **profitable vs losing trades** by sentiment using Seaborn bar charts.

### 2️⃣ Do traders take **more risk** when the market is greedy?

- Analyzed trade sizes using `size usd` and categorized them into **Small / Medium / Large** buckets.
- Compared risk-taking behavior by plotting trade size distributions across market sentiment.

### 3️⃣ Are some traders **better in fearful markets** than others?

- Aggregated each trader’s PnL during Fear vs Greed using pivot tables.
- Identified "Fear Experts" – traders who consistently earned profits during fearful conditions.
- Visualized individual trader performance using heatmaps and ranking charts.

---

## 📊 Visualizations

The notebook includes:
- 📈 Bar plots comparing average PnL across sentiments
- 📉 Boxplots showing trade size distributions
- 🔥 Heatmaps of trader performance by sentiment
- ✅ Side-by-side charts for Profit vs Loss percentages

All visualizations are built using `matplotlib` and `seaborn`.

---

## 🧹 Data Preprocessing Steps

- Converted Unix timestamps to readable `datetime`.
- Merged datasets on aligned timestamps (`time`).
- Engineered new features:
  - `pnl_flag` → Profit / Loss / Neutral
  - `size_bucket` → Small / Medium / Large
  - `sentiment_strength` → Extreme Fear, Fear, Greed, Extreme Greed

---

## 🚀 Technologies Used

- `Python 3.x`
- `Pandas`
- `Seaborn`
- `Matplotlib`
- `Jupyter Notebook`

---

## 📁 Files in This Repository

| File | Description |
|------|-------------|
| `trader_sentiment_analysis.ipynb` | Main notebook with full analysis, visualizations, and insights |
| `merged_cleaned_data.csv` | Final processed dataset (if included) |
| `README.md` | This documentation file |

---

## 📬 How to Apply

As part of the assignment process, please send this completed analysis with your resume to:

📧 **saami@bajarangs.com**, **nagasai@bajarangs.com**  
📩 CC: **sonika@primetrade.ai**  
📌 Subject: `"Junior Data Scientist – Trader Behavior Insights"`

---

## 🏁 Conclusion

This project offers insights into how **emotions drive trading decisions**, and how certain traders may have an edge during **market downturns**. It bridges behavioral finance with real trading outcomes — an exciting intersection of psychology and crypto analytics.

---

