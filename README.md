# 📊 Sales & Order Analytics Dashboard

An end-to-end data analytics project featuring data preparation using **Python (Pandas)**, followed by an interactive, enterprise-grade dashboard designed in **Power BI**.

---

## 📌 Project Overview
This project analyzes an e-commerce dataset containing 1,200 unique customer orders. The objective was to clean the transaction logs, address operational inefficiencies, and deliver actionable insights regarding product performance, marketing channels, and order fulfillment.

### 🔑 Key Metrics (KPIs)
* **Total Revenue:** $1.26M
* **Total Orders:** 1.2K (1,200 Orders)
* **Unique Products:** 7 Types
* **Payment Methods:** 5 Types
* **Average Order Value (AOV):** $1.05K

---

## 🛠️ Tech Stack & Workflow

### Phase 1: Data Cleaning & Feature Engineering (Python)
Using a customized Python script (`Pandas`), the raw file `Dataset for Data Analytics(Sheet1).csv` was processed to ensure top-tier data quality before visualization:
* **Missing Values Handling:** Filled missing values in `CouponCode` with a standard `'No Coupon'` string for seamless dashboard filtering.
* **Temporal Disaggregation:** Converted the text-based `Date` column into a proper `datetime` index, extracting the `YearMonth` feature for historical trend analysis.
* **Financial Auditing:** Cross-validated the `TotalPrice` against the calculation ($Quantity \times UnitPrice$) to confirm 100% data integrity.

### Phase 2: Interactive Data Visualization (Power BI)
Imported the cleaned dataset into Power BI Desktop, applied a customized modern theme, and engineered a rich analytical view:
* **Revenue by Product:** Evaluated top-grossing items, identifying **Chairs** and **Printers** as primary revenue drivers.
* **Order Status Distribution:** Implemented a categorical Donut Chart highlighting operational workflow distribution.
* **Revenue by Year and Month:** Embedded a monthly sales line chart to trace historical order pacing and demand fluctuations.
* **Revenue by Referral Source:** Segmented total revenue by marketing channels using an interactive Treemap view.
* **Interactive Slicers:** Added three dynamic filters for **Month Name**, **CouponCode**, and **PaymentMethod** to allow comprehensive data drilling.

---

## ⚠️ Critical Business Insights Discovered
* **The 41% Fulfillment Bottleneck:** Analytics revealed a severe operational risk—**over 41% of all placed orders result in either Cancellation (20.83%) or Returns (20.58%)**. This critical insight advises immediate quality control audits on delivery pipelines.
* **Marketing Efficiency:** Social campaigns driven by **Instagram** and **Email** outperformed other channels, marking them as the most profitable ad spend destinations.

---

## 📂 Repository Structure
```text
├── Dataset for Data Analytics(Sheet1).csv  # Raw data log
├── data_preparation.py                     # Python ETL cleaning script
├── Cleaned_Dataset_for_PowerBI.csv         # Cleaned output for BI
├── Sales_Analytics_Dashboard.pbix          # Power BI project file
└── README.md                               # Project documentation
