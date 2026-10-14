# Excel Dashboards

Two Excel workbooks built with Pivot Tables, Slicers and a summary dashboard sheet.

Dashboard 1
<img width="860" height="398" alt="Debit-Credit_card_Image" src="https://github.com/user-attachments/assets/ef63b1dc-1144-453b-8643-62cf58faf738" />

Dashboard 2
<img width="930" height="469" alt="Bank_Dashboard_image" src="https://github.com/user-attachments/assets/4821d476-459b-4b1d-bcdd-ef7ec0548841" />


## 1. Debit & Credit Transaction Analysis
**File:** `Debit_and_Credit_banking_data_new_2_.xlsx`

**Goal:** Compare credits against debits across branches, banks and months, and flag high-risk transactions.

**Data:** 100,000 transactions (Jan to Dec 2024, INR), 6 branches, 6 banks, 3 transaction methods (Credit Card, Debit Card, Bank Transfer).

**Workbook contents**
- `Credit_Debit_Data`: raw data
- Question sheets 1 to 12 with Pivot Tables, including High-Risk vs Normal and suspicious-transaction analysis
- `DASHBOARD`: summary sheet with Slicers

![Debit & Credit Excel Dashboard](../images/debit_credit_excel_dashboard.png)

### Key Insights
- **Money in and money out are almost perfectly balanced.** Total credits were about ₹127.6M against debits of about ₹127.3M, a net inflow of only about ₹0.32M (roughly 0.25% of credit volume).
- **East Branch had the strongest net inflow (+₹355K), while Main Branch had the largest net outflow (-₹246K).** City Center was also net negative (-₹75K). Main Branch is the one to watch for outflow pressure.
- **Net flow swings month to month.** May had the highest net inflow (+₹559K) and April the largest net outflow (-₹513K). Of the 11 full months, 6 were net inflow and 5 net outflow. December has only 305 transactions because the data ends on 1 December, so it should be excluded from trend comparisons.
- **About 10.4% of transactions (10,428) are flagged High Risk** (amount of ₹4,500 or more). The flag covers the top slice of an amount range that tops out at about ₹5,000, and the average transaction is only about ₹2,549.
- **High-risk share is similar everywhere.** City Center and East Branch are highest at about 11%, the other branches about 10%. By bank, Axis Bank is highest at 10.8% and State Bank of India lowest at 10.2%.
- **Transaction method makes no real difference.** Volume is split evenly (about 33.3K each) and the high-risk share is 10.3% to 10.5% for Bank Transfer, Credit Card and Debit Card, so risk is not concentrated in one channel.
- **Debit transactions carry a slightly higher high-risk share than credits** (10.5% vs 10.4%).

---

## 2. Bank Loan Portfolio Analysis
**File:** `dashboard.xlsx`

**Goal:** Track the health, revenue and risk of a loan portfolio across states, regions, branches and borrower groups.

**Data:** About 65.5K loan accounts (FY2017 to FY2020), 16 states, 112 branches, 11 regions, total loan amount of about ₹751M.

**Workbook contents**
- `Banking Data`: raw data
- Pivot Table sheets: `1 to 7`, `8 to 10`, `11 to`
- `Branch Wise Analsis`
- `Dashboard`: summary sheet with Slicers

![Loan Excel Dashboard](../images/loan_excel_dashboard.png)

### Key Insights
- **The portfolio is concentrated geographically.** Uttar Pradesh, Punjab and Bihar make up about 47% of the ₹751M loan value, and the top 5 states (adding Haryana and Rajasthan) about 67%. Ludhiana is the largest region (₹129M) and Mathura the largest branch by loan value.
- **Total revenue (interest + fees) is about ₹156.5M**, roughly 21% of the loan amount.
- **Default is low, delinquency is not.** Only 1,020 loans (about 1.6%) are in default, but 7,106 (about 10.8%) are delinquent. Delinquency is about 10% to 11% in almost every state, so it is a portfolio-wide issue rather than a regional one. Varanasi (12%) and Jalandhar branch (14%) are the highest.
- **Credit grade is the strongest risk signal.** Delinquency climbs from about 4% for Grade A to 9% (B), 14% (C), 17% (D and E), 22% (F) and 26% (G).
- **Lower grades earn more per rupee lent.** Revenue as a share of loan amount rises from about 10% for Grade A to about 37% for Grade G, so the higher-risk grades are the ones that also bring in the most return.
- **60-month loans drive revenue.** They are about 42% of loan value but about 59% of revenue (₹91.7M of ₹156.5M).
- **Borrowers aged 26 to 45 are the core base**, with about 67% of loan value. The 56 to 63 group is small (1,656 accounts) but has the highest default rate at roughly 7%, against 1% to 2% for other age groups.
- **Home loans lead.** They make up about 37% of loan value, and the top 3 purposes (Home Loan, Services, Business) about 69%. Home Loan, Services and Business are the main revenue sources.
- **Verification status does not predict risk.** Delinquency is about 11% for Verified, Source Verified and Not Verified loans alike, so the current verification step is not separating good borrowers from bad.
- **Borrowers are almost entirely women** (65,511 of 65,535 loans with a recorded gender).
- **Disbursement peaked in FY2019**, which accounts for about 57% of loan value. 55.5% of loans are still active and about 0.9% are NPA or written off.

## Skills Demonstrated
Pivot Tables, Slicers, dashboard design, KPI reporting, risk and segmentation analysis

## How to Open
Download the file and open it in desktop Microsoft Excel. Pivot Tables and Slicers don't work in the browser preview.
