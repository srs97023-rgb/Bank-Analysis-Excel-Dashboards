# Banking Analytics Dashboards | Excel & Tableau

Two end-to-end banking analytics projects, each built twice: once in **Excel** (Pivot Tables, Slicers, dashboard sheet) and once in **Tableau** (calculated fields, KPI worksheets, final dashboard).

| # | Project | Dataset | Excel | Tableau |
|---|---------|---------|-------|---------|
| 1 | Debit & Credit Transaction Analysis | 100,000 transactions (2024) | `Debit_and_Credit_banking_data_new_2_.xlsx` | `DEBIT_AND_CREDIT_BANKING_DATA_1.twbx` |
| 2 | Bank Loan Portfolio Analysis | ~65.5K loan accounts (FY2017-FY2020) | `dashboard.xlsx` | `Tableau_Bank_Analysis_Project.twbx` |

---

## Project 1: Debit & Credit Transaction Analysis

**Goal:** Understand how money moves through the bank, compare credits against debits, and flag high-risk and suspicious transactions.

### Dataset
- **100,000 transactions** from Jan to Dec 2024, in INR
- 6 branches (Main, City Center, Suburban, North, East, Downtown)
- 3 transaction methods: Credit Card, Debit Card, Bank Transfer
- Columns: Customer ID, Customer Name, Account Number, Transaction Date, Transaction Type, Amount, Balance, Description, Branch, Transaction Method, Currency, Bank Name, Week Start, High-Risk Flag

### Quick facts
- About 50/50 split between credit (50,028) and debit (49,972) transactions
- Total credits of about ₹127.6M against total debits of about ₹127.3M
- About 10.4% of transactions are flagged **High Risk** (amount of ₹4,500 or more)

### Metrics built
- Total Credit Amount, Total Debit Amount, Net Transaction Amount
- Credit-to-Debit Ratio
- Total Transactions and Account Activity Ratio
- Branch Growth % (period-over-period change in amount)
- High-Risk Transaction Flag (High Risk vs Normal)

### Excel version
- 12 question-wise analysis sheets (Question 1 to 12) built with Pivot Tables
- Interactive Slicers
- Summary `DASHBOARD` sheet
- High-Risk vs Normal and suspicious-transaction analysis

### Tableau version
- 14 worksheets (Question 1 to 12, plus sub-parts) combined into a **FINAL DASHBOARD**
- Calculated fields for all metrics above

**Dashboard preview**

![Excel Dashboard - Debit & Credit](images/debit_credit_excel_dashboard.png)
![Tableau Dashboard - Debit & Credit](images/debit_credit_tableau_dashboard.png)

**Live Tableau dashboard:** _add your Tableau Public link here_

---

## Project 2: Bank Loan Portfolio Analysis

**Goal:** Track the health of a loan portfolio by looking at loan volume, revenue, delinquency, default and borrower profile across states, branches and regions.

### Dataset
- **~65.5K loan accounts** across 16 states, 112 branches and 11 regions
- Disbursements from FY2017 to FY2020, with total loan amount of about ₹751M
- 52 columns, including State, Branch, Region, Client, Age, Gender, Home Ownership, Loan
