# 📈 Risk & Pricing Analytics Using Python

**Python | Predictive Modeling**
**JPMorgan Chase & Co. – Quantitative Research Virtual Experience (Forage)**

---

## 📌 Project Overview

This project was completed as part of the **JPMorgan Chase & Co. Quantitative Research Virtual Experience Program on Forage**. The objective was to apply data analysis and predictive modeling techniques to **realistic financial and risk management problems**, supporting decision-making in trading, storage pricing, and credit risk assessment.

The work spans **time-series analysis**, **contract pricing**, and **probability of default modeling**, with a strong emphasis on translating data into **business-relevant outputs**.

---

## 🛢️ Part 1: Natural Gas Price Analysis & Extrapolation

### 🧠 Business Context

The trading desk receives **monthly snapshots of natural gas prices** from a market data provider, representing prices at the end of each calendar month. The available data spans from **October 2020 to September 2024**, with limited forward visibility.

The desk requested:

* A clear visualization of historical price behavior
* An approach to estimate prices on arbitrary dates
* A **one-year extrapolation** to support longer-term storage contracts

---

### 📊 Analysis Approach

* Loaded and explored historical price data from CSV
* Visualized monthly prices to identify **trend and seasonality**
* Modeled prices using:

  * Linear regression for long-term trend
  * Sinusoidal functions to capture **annual seasonal variation**
* Built a reusable function that:

  * Takes a date as input
  * Returns an estimated gas price (historical or future)

---

### 💡 Key Insights

* Natural gas prices exhibit a **clear annual seasonal pattern**
* Prices trend upward over the observed period
* Seasonal demand (e.g., winter heating) is a major driver of volatility

---

## 💰 Part 2: Gas Storage Contract Pricing Model

### 🧠 Business Context

A client wants to purchase gas during low-price periods, store it, and sell it later when prices increase. The trading desk needed a **pricing model** to evaluate whether such a storage contract is profitable once all costs are considered.

---

### ⚙️ Pricing Model Design

A Python function was built to calculate the **value of a gas storage contract**, accounting for:

* Injection dates and purchase prices
* Withdrawal dates and selling prices
* Injection and withdrawal rate limits
* Maximum storage capacity
* Monthly storage fees
* Injection and withdrawal costs

The model computes:

* Cash outflows from purchasing and injecting gas
* Cash inflows from selling gas
* Total storage and operational costs
* Net contract value (profit or loss)

---

### 💡 Business Outcome

* Enables scenario testing for different injection/withdrawal strategies
* Provides a transparent, auditable pricing logic
* Can be extended and validated for production use

---

## 🏦 Part 3: Credit Risk & Probability of Default Modeling

### 🧠 Business Context

The retail banking arm was experiencing higher-than-expected default rates on personal loans. The risk team wanted to **predict the probability of default (PD)** for borrowers in order to estimate expected losses and set aside adequate capital.

---

### 📊 Predictive Modeling

* Loaded borrower-level loan data
* Engineered financial ratios:

  * Debt-to-income
  * Payment-to-income
* Trained a **logistic regression model** to predict default probability
* Evaluated model performance using ROC and AUC metrics
* Estimated **expected loss**, assuming a fixed recovery rate

---

### 💡 Key Insight

Borrower characteristics such as **credit score, debt burden, and employment history** are strong indicators of default risk and can be used to guide loss provisioning.

---

## 📉 Part 4: FICO Score Bucketing via Quantization

### 🧠 Business Context

Mortgage risk models required **categorical inputs**, but FICO scores span a wide numeric range (300–850). The risk team requested an optimal method to convert raw scores into **credit rating buckets**.

---

### 🧮 Methodology

* Implemented a **quantization approach** to bucket FICO scores
* Used a **log-likelihood optimization framework**
* Applied **dynamic programming** to find bucket boundaries that best summarize default behavior
* Ensured the approach generalizes to future datasets

---

### 💡 Business Outcome

* Produced data-driven FICO rating buckets
* Improved interpretability of credit risk
* Enabled compatibility with categorical-model architectures

---

## 🛠 Tools & Technologies

* **Python** (Pandas, NumPy, Matplotlib, Scikit-learn)
* **Excel** (loan and price datasets)

---

## 📂 Repository Contents

* Python scripts for:
  * Price analysis & extrapolation
  * Storage contract pricing
  * Probability of default modeling
  * FICO score bucketing
* Excel datasets used for analysis
* Certificate of completion

---

## 🎓 Certification

**JPMorgan Chase & Co. – Quantitative Research Virtual Experience (Forage)**
*Completed January 2026*

Skills demonstrated:

* Time-series analysis & forecasting
* Pricing and cash-flow modeling
* Predictive analytics & classification
* Risk analysis and data-driven decision-making

---
