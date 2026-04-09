# 📊 Customer Segmentation & Revenue Leakage Analysis Using RFM and K-Means

## 🧠 Overview

This project aims to analyze customer behavior and identify key business opportunities using a data-driven approach. By combining **RFM (Recency, Frequency, Monetary) analysis** with **K-Means clustering**, this project uncovers:

* High-value customers driving revenue
* Customers at risk of churn
* Revenue loss caused by product returns (*revenue leakage*)

The goal is to provide actionable insights to improve **customer retention, operational efficiency, and profitability**.

---

## 🎯 Business Problem

Companies often focus on increasing sales but overlook:

* Which customers actually drive the most revenue
* Which customers are at risk of leaving
* How much revenue is lost due to returns

This project answers:

> How can we segment customers and reduce revenue loss to improve overall business performance?

---

## 📂 Dataset

* Online Retail Dataset
* Contains transactional data including:

  * CustomerID
  * InvoiceDate
  * Quantity
  * UnitPrice

---

## 🔍 Analysis Workflow

### 1️⃣ Data Cleaning

* Removed missing CustomerID
* Filtered negative/invalid transactions
* Created TotalPrice feature

---

### 2️⃣ Return Analysis

* Identified customers with high return quantity and value
* Found extreme imbalance where a small number of customers dominate returns

👉 **Insight:**
A small group of customers contributes disproportionately to returns, leading to potential revenue leakage.

---

### 3️⃣ Purchase Analysis

* Analyzed total purchase quantity and value per customer
* Identified high-value customers

👉 **Insight:**
Revenue is heavily concentrated among a small number of customers (**customer concentration risk**).

---

### 4️⃣ Revenue Leakage Analysis

* Calculated total revenue vs returned value

👉 **Key Finding:**
~**6–7% of total revenue is lost due to returns**

👉 **Business Impact:**
Reducing even 1–2% leakage can significantly improve profit without increasing sales.

---

### 5️⃣ RFM Analysis & Segmentation

Customers segmented based on:

* Recency → how recently they purchased
* Frequency → how often they purchase
* Monetary → how much they spend

👉 **Segments Identified:**

* Champions (high value, loyal)
* Regular Customers
* At Risk
* Big Spenders
* New Customers

---

### 6️⃣ Clustering (K-Means)

* Applied log transformation to handle skewed data
* Used Elbow Method & Silhouette Score
* Optimal cluster: **k = 3**

---

### 7️⃣ Cluster Profiling

| Cluster   | Characteristics                        | Business Meaning   |
| --------- | -------------------------------------- | ------------------ |
| Cluster 1 | Low Recency, High Frequency & Monetary | 🔥 Loyal Customers |
| Cluster 0 | متوسط values                           | Regular Customers  |
| Cluster 2 | High Recency, Low Frequency & Monetary | ⚠️ Churn Risk      |

👉 **Insight:**
Customers can be grouped into 3 actionable segments for targeted strategies.

---

## 💡 Key Business Insights

* 📌 Revenue is dominated by a small group of high-value customers
* ⚠️ A small number of customers cause significant revenue leakage
* 📉 Some customers are at high risk of churn
* 📈 Majority of customers are "Regular" → biggest growth opportunity

---

## 🚀 Business Recommendations

### 🎯 Retain High-Value Customers

* Loyalty programs
* Personalized offers

### ⚠️ Reduce Revenue Leakage

* Monitor high-return customers
* Improve product quality & logistics

### 🔄 Re-engage At-Risk Customers

* Marketing campaigns
* Discounts / reminders

### 📈 Grow Regular Customers

* Upselling & cross-selling strategies

---

## 🧾 Conclusion

This analysis shows that:

* Revenue is not evenly distributed across customers
* A portion of revenue is lost due to returns
* Customer segmentation enables targeted and efficient strategies

👉 By leveraging these insights, companies can:

* Increase profitability
* Reduce operational inefficiencies
* Make better business decisions

---

## 🛠️ Tech Stack

* Python (Pandas, NumPy)
* Data Visualization (Matplotlib, Seaborn)
* Machine Learning (Scikit-learn)

---

## 📌 Author

**Yopi Ibra**
Aspiring Data Scientist | Focused on Business & Manufacturing Analytics

---

## ⭐ Why This Project Matters

This project demonstrates the ability to:

* Translate data into business insights
* Apply machine learning for real-world problems
* Think beyond models and focus on **business impact**

---

