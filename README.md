# 💳 Banking Risk Analytics Dashboard using Power BI

## 📌 Project Overview

This project demonstrates how **risk analytics** can be applied in the **banking and financial sector** to reduce lending risks. The Power BI dashboard helps visualize client banking behavior, deposits, loans, and fees, enabling data-driven decisions on whether to approve or reject loan applications.

---

## 🧹 Data Cleaning & Preparation

- Created `Engagement Timeframe` column to represent client-bank duration.
- Created `Engagement Days` column using `DATEDIFF`.
- Created `Income Band` column using bins for estimated income.
- Calculated `Processing Fees` based on the Fee Structure.

---

## 🧮 DAX Calculations

### Aggregates
- `Bank Deposit = SUM('Clients - Banking'[Bank Deposits])`
- `Total Clients = DISTINCTCOUNT('Clients - Banking'[Client ID])`
- `Total Fees = SUMX('Clients - Banking', [Total Loan] * [Processing Fees])`

### KPI Metrics
- **Total Clients**
- **Total Loan** = Bank Loan + Business Lending + Credit Card Balance
- **Total Deposit** = Bank Deposit + Savings + Checking + Foreign Currency
- **Credit Card Balance**
- **Engagement Length (Days)**

---

## 📊 Dashboard Views

- **Home Dashboard**: Overview of all key metrics
- **Loan Analysis**: Breakdown of loans by type, gender, advisor, etc.
- **Deposit Analysis**: Insights into various deposit types


---

## ✅ Key Insights

- Identify clients likely to repay or default on loans
- Understand deposit behaviors across account types
- Determine which client segments carry higher risks
- Compare client engagement across bank types (e.g., Private vs. Public)
