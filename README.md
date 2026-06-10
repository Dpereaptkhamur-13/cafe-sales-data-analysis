# Cafe Sales Data Pipeline & Interactive Dashboard

## 📌 Project Overview
This project demonstrates an end-to-end data engineering and analytics solution. I took a raw, heavily corrupted dataset consisting of over 9,900+ cafe transaction records and built a systematic cleaning pipeline to restore data integrity, culminating in an interactive business intelligence dashboard.

---

## 🛠️ Data Cleaning Challenges & Solutions

Real-world data is messy, and this dataset was a prime example. Here is how I handled the primary structural and logical anomalies:

* **Mathematical Anomaly Realignment:** Identified transaction rows where quantities were glitched to `0` but active totals existed. Successfully reverse-engineered the actual purchasing volume using division arrays ($$\text{Total Spent} \div \text{Price Per Unit}$$).
* **Structural String Shifts:** Resolved instances where system error text blocks (like `"Unspecified $3 Item"`) shifted into the wrong categorical columns (**Location** and **Transaction Date**).
* **Metadata Normalization:** Managed corrupted logs by classifying missing text parameters into a standardized `"Unknown"` placeholder category, successfully preserving overall financial and revenue data integrity.
* **Calculation Automation:** Built out a fully verified, hardcoded evaluation array to calculate and lock exact tracking metrics across all 9,999+ data rows.

---

## 📊 The Dynamic Dashboard
The final interactive dashboard was engineered entirely **macro-free** using linked native **Slicers**, **Pivot Tables**, and synchronized **Pivot Charts**. 


### Dashboard Preview:
<img width="1312" height="797" alt="image" src="https://github.com/user-attachments/assets/942297bb-cf78-455b-ac62-d6c1a8e3c6ad" />


---

## 🚀 How to Explore This Project
1. Download the `dirty_cafe_sales.xlsx` workbook from this repository.
2. Open the file in Microsoft Excel.
3. Navigate to the `Sheet1` tab to interact with the slicers and watch the entire analytical layout dynamically update in real-time.
