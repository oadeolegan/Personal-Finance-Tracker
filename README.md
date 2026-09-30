# Personal-Finance-Tracker
End-to-end data cleaning and Power BI dashboard analyzing 8,000+ personal financial transactions
[Personal-Finance-Tracker.md](https://github.com/user-attachments/files/32843313/Personal-Finance-Tracker.md)
# Personal Finance Tracker: Bank Statement Analysis (Aug 2023 – May 2026)

An interactive Power BI dashboard and data cleaning project analyzing multi-year transactional cash flows, fund allocations, and operational spending patterns.

---

## 📌 Project Overview
This project processes nearly three years of raw banking statement data (August 2023 to May 2026) to provide clear visibility into historical inflows, outflows, internal transfers, and distinct spending categories. 

The dashboard segregates personal living expenses from operational disbursements (such as fuel procurement, sound maintenance, and community logistics), tracking cumulative totals and category-specific allocations.

---

## 📊 Dashboard Preview
<img width="1006" height="745" alt="image" src="https://github.com/user-attachments/assets/58cd50b8-6feb-47d5-ac2e-7e414eeca3d3" />


---

## 🛠️ Tools & Technologies
- **Microsoft Excel:** Raw statement ingestion, column-level filtering, record sorting, removal of redundant statement rows, and category assignment.
- **Power BI Desktop:** Data modelling, custom DAX metrics, KPI card formatting, and dark-themed visualization.
- **Key Concepts:** Transaction classification, cash flow tracking, operational expense separation.

---

## 📈 Key Metrics & Summary Findings
- **Total Credit Analyzed:** ₦17.22M
- **Total Debit Analyzed:** ₦16.88M
- **Net Balance:** ₦339.21K
- **Highest Volume Category:** Internal Transfers (₦5.72M Credit / ₦5.01M Debit)
- **Top Outflow Drivers:**
  - **Church – Fuel:** ₦5.22M
  - **Internal Transfers:** ₦5.01M
  - **Personal – Miscellaneous Outflow:** ₦4.79M
  - **Food Purchase:** ₦984.94K
  - **Church Operations & Logistics:** ₦237.45K

---

## 🔍 Data Pipeline & Workflow

### 1. Data Cleaning & Preparation (Microsoft Excel)
- **Audit & Extraction:** Filtered raw bank statement exports across 2023–2026, eliminating redundant headers, null entries, and balance checkpoint lines.
- **Inspection & Sorting:** Used column filters to review varied bank narrative strings, flags, and transaction remarks.
- **Category Normalization:** Standardized transaction records into dedicated categories, distinctly separating personal expenses (e.g., *Food Purchase, Subscriptions & Airtime, Upkeep*) from organizational/logistical disbursements (e.g., *Church - Fuel, Engine Oil, Sound Maintenance*).

### 2. Modelling & DAX Measures (Power BI)
- Loaded cleaned transactional tables into Power BI and created calculated measures to monitor net balances, inflow totals, and debit distributions:
  - `Total Credit = SUM(Transactions[Credit])`
  - `Total Debit = SUM(Transactions[Debit])`
  - `Net Balance = [Total Credit] - [Total Debit]`
- Created multi-level slicers for dynamic filtering across **Category**, **Channel**, **Year**, and **Month**.

### 3. Visual Layout & Reporting Layer
- **Executive KPI Cards:** Instant visibility into aggregate Credits, Debits, Net Position, and Top Volume Category.
- **Donut Chart (Credit by Category):** Highlights major funding sources, including *Church Ops & Logistics* (38.79%), *Internal Transfers* (33.22%), and *Personal Inflow* (19.85%).
- **Ranked Bar Chart (Debit by Category):** Outlines total expenditure ranked by volume, clearly showing recurring operational costs alongside living expenses.

---

## 📬 Contact
- **Name:** Olusi Joseph Adeolegan
- **Email:** olusijosephadeolegan@gmail.com
- **Phone:** +234 902 380 9732
- **LinkedIn:** www.linkedin.com/in/joseph-olusi-128908326
