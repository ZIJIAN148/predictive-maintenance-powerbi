# 🏭 Predictive Maintenance & OEE Dashboard (Power BI)

## 📌 Executive Summary
This project analyzes manufacturing telemetry to predict mechanical failures and optimize Overall Equipment Effectiveness (OEE). By modeling real-time sensor data (torque, RPM, tool wear), the dashboard identifies critical failure thresholds, enabling data-driven preventative maintenance strategies.

![Dashboard Preview](dashboard-screenshot.png)

---

## ⚙️ Methodology & Tech Stack

| Phase | Tool | Actions Performed |
| :--- | :--- | :--- |
| **Data Ingestion & Cleaning** | **Excel (Power Query)** | Extracted and transformed 10,000+ rows of raw CNC machine sensor logs, filtering anomalies. |
| **Data Modeling** | **Power BI** | Engineered a Star Schema relational model separating machine facts from product quality dimensions. |
| **Calculation & Logic** | **DAX** | Wrote dynamic measures to calculate real-time Failure Rates and Average Tool Wear. |
| **Visualization** | **Power BI** | Developed an interactive management dashboard highlighting the physical operational envelope. |

---

## 📊 Core Insights & Strategic Value

* **Identifying the Failure Threshold:** The data model reveals that catastrophic machine failures cluster heavily when tool wear reaches the 200–220 minute mark.
* **Strategic Recommendation:** Implementing a strict preventative maintenance protocol to automatically swap cutting tools at 190 minutes will slightly increase upfront tooling costs but virtually eliminate unpredictable line downtime, maximizing total OEE.
* **Quality Impact:** Low-quality product variants account for the highest volume of machine stress and subsequent failures.

---

## 📂 Repository Contents
* `predictive_maintenance.pbix`: The full Power BI file containing the data model and DAX measures.
* `ai4i2020.csv`: The underlying manufacturing dataset.
* `dashboard-screenshot.png`: High-resolution visual output of the final dashboard.
