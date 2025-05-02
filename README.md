# 📈 Investigating Deepseek’s Influence on Public Sentiment and Tech Stock Performance

## 🧠 Real-World Problem

In January 2025, the release of **DeepSeek-R1**, a Chinese open-source LLM, triggered a notable shift in public attention toward AI technology. The release coincided with a **temporary drop in NVIDIA's stock price**, raising an important question:

> Can sudden bursts of public attention around emerging AI technologies influence stock market performance, especially for companies like NVIDIA and Microsoft?

This project aims to assess **whether online sentiment and search attention translate into financial movement** in public markets, using data-driven methods.

---

## 🔍 Project Scope

- **Sentiment & Attention Analysis**
  - Twitter data: tweet count and average sentiment
  - Google News headlines
  - Google Trends search volume for “Deepseek”
  
- **Stock Price Movement**
  - Daily returns and closing prices for:
    - NVIDIA (NVDA)
    - Microsoft (MSFT)

- **Quantitative Methods**
  - Correlation & regression analysis
  - Lag analysis and Granger causality tests
  - Time series decomposition and visualization

---

## 🛠 Technologies Used

- **Language:** R (R Markdown)
- **Libraries:** `dplyr`, `ggplot2`, `forecast`, `quantmod`, `sentimentr`, `zoo`, `lubridate`
- **Data Sources:**
  - Custom tweet/news dataset
  - Google Trends API
  - Yahoo Finance (via `quantmod`)

---

## 📊 Key Findings

- **Tweet Volume vs NVDA Return:** A modest **positive same-day correlation**
- **Average Sentiment:** Weak or inconsistent correlation with returns
- **Lag Analysis:** No significant delayed effect found (Granger causality)
- **Regression Results:** Tweet volume is a significant predictor for NVDA; less so for MSFT
- **Hypothesis Testing:** High attention days showed marginally higher NVDA returns

> These results suggest that attention spikes like Deepseek’s release can briefly sway markets, particularly for companies directly associated with AI infrastructure.

---

## 📁 Project Structure

```
.
├── final_optimized.Rmd     # Optimized R Markdown analysis
├── data/                   # CSV files for tweet/news data
└── README.md               # This file
```

---

## 🚀 Running the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/deepseek-stock-impact.git
   ```

2. Open `final_optimized.Rmd` in RStudio

3. Install required packages if needed:
   ```r
   install.packages(c("dplyr", "ggplot2", "forecast", "quantmod", "sentimentr", "zoo", "lubridate"))
   ```

4. Knit to HTML to view full analysis and charts

---

## 📌 Future Improvements

- Include sentiment from Reddit and LinkedIn
- Use more advanced models (e.g., XGBoost, LSTM)
- Apply the methodology to other major AI events (e.g., GPT releases)

---

## 🔗 Report Link

An interactive HTML version of the report is available [here](https://grand-pixie-2256f8.netlify.app/).

---



