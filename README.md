# 💼 JP Morgan Quantitative Research Virtual Experience

This repository contains solutions to all tasks from the **J.P. Morgan Quantitative Research Virtual Experience** offered by [Forage](https://www.theforage.com/). The program simulates real-world responsibilities of a **Quantitative Analyst**, combining statistical modeling, financial forecasting, and credit risk analysis in a hands-on format.

Each task was designed to mirror analytical workflows used in quantitative research at leading financial institutions.

---

## 📁 Contents

### 📈 Task 1 – Forecasting Natural Gas Prices

**Objective:**  
Forecast monthly natural gas prices using historical data to support contract pricing and market analysis.

**Approach:**  
- Cleaned and resampled monthly price data, handling missing values through interpolation  
- Implemented the **Holt-Winters Exponential Smoothing** model with additive trend and seasonality  
- Evaluated forecast accuracy using MAE, RMSE, and MAPE  
- Visualized historical vs. predicted price movements to assess model validity

**Outcome:**  
A reliable time-series forecasting pipeline suitable for pricing long-term gas contracts or scenario testing.

---

### 📦 Task 2 – Storage Contract Pricing Model

**Objective:**  
Design a flexible tool to calculate the **profitability of buying, storing, and reselling** natural gas across months.

**Approach:**  
- Used the forecasted prices from Task 1 to simulate future buy/sell price scenarios  
- Developed a **contract pricing function** that takes injection/withdrawal dates, volumes, storage costs, and capacity as inputs  
- Modeled real-world constraints like injection/withdrawal fees and monthly holding costs

**Outcome:**  
A reusable simulation tool to support trading desks in estimating fair storage contract values under different market conditions.

---

### 🧮 Task 3 – Credit Risk Analysis & Expected Loss Modeling

**Objective:**  
Predict loan default probability and compute **expected credit losses** using customer-level data.

**Approach:**  
- Trained **Logistic Regression** and **Random Forest** classifiers on borrower features (e.g., income, debt, credit history)  
- Evaluated models using classification report, confusion matrix, and **ROC-AUC**  
- Computed **Expected Loss (EL)** using:  
  **Expected Loss (EL)** = **PD** × **Exposure at Default (EAD)** × *(1 - Recovery Rate)*

**Outcome:**  
An interpretable, production-ready PD/EL calculator that can assist in provisioning and credit decision automation.

---

### 📊 Task 4 – FICO Score Bucketing for Risk Modeling

**Objective:**  
Convert continuous **FICO scores** into discrete risk buckets to enable classification models to better capture credit risk.

**Approach:**  
Implemented and compared three bucketing strategies:
1. **Quantile Binning** – evenly distributes borrowers across score percentiles
2. **KMeans Clustering** – data-driven grouping based on score patterns
3. **Log-Likelihood Optimization**   
   - Maximizes the ability to distinguish defaults across buckets  
   - Produces risk segments aligned with business interpretability

**Outcome:**  
A validated segmentation strategy ready for integration into scorecards, PD models, or credit policy systems.

---

## ⚙️ Tools & Libraries Used

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Statsmodels, Scikit-learn, OptBinning
---

##  Summary

Through this program, I applied statistical techniques and Python programming to solve real-world problems in **credit risk**, **financial forecasting**, and **contract valuation** — reinforcing my interest in data-driven policy and finance.

---

📂 **View full project notebooks in this repository**  
💬 **Feel free to connect or reach out for collaboration or discussion!**

