# 💳 Loan Cashflow & Credit Risk Analytics

![Dashboard](images/DASHBOARD%20LOAN.png)

Banking analytics project focused on loan cashflow analysis, lending portfolio monitoring, and credit risk analytics using SQL Server and Power BI.

This project simulates how banks analyze lending profitability, portfolio quality, and credit risk through cashflow modeling and portfolio monitoring.

---

## 🧠 Business Problem

Banks need to answer several critical questions related to lending performance and portfolio risk:

- How do loans generate cashflow and profitability over time?
- Which customer segments contain higher credit risk exposure?
- How do prepayment and default impact interest income?

The project focuses on evaluating the relationship between lending growth, profitability, and portfolio risk.

---

## ⚠️ Challenges

- Loan cashflow data is fragmented across individual loan contracts
- Difficult to simultaneously monitor:
  - Principal
  - Interest
  - Outstanding Balance
- Limited visibility into:
  - Dynamic credit risk
  - Portfolio quality trends over time

---

## 🎯 Objectives

- Model loan cashflow and amortization schedule
- Calculate interest income over time
- Monitor outstanding balance
- Monitor credit risk indicators:
  - NPL
  - Delinquency
- Build what-if scenarios:
  - Prepayment
  - Default

---

## 🏗️ Data Architecture

```text
HOPDONG_TINDUNG
KHACHHANG
KHACHHANG_TRANO
DUNO_KH
        ↓
Stored Procedure (Cashflow + Outstanding Calculation)
        ↓
SQL View (Data Modeling)
        ↓
Power BI Dashboard (Portfolio Monitoring & Risk Analysis)
```

---

## ⚙️ Technical Highlights

### SQL Server

- Built amortization schedule logic
- Calculated:
  - Principal cashflow
  - Interest cashflow
  - Outstanding balance over time

---

### SQL Techniques

- CTE
- Window Function
- Aggregation
- Conditional Logic

---

### Data Modeling

#### Star Schema

- Dim Date
- Dim Customer
- Dim Loan
- Fact Payment

---

### Power BI Development

- Data Modeling
- Risk Monitoring Dashboard
- Lending Portfolio Visualization
- Scenario Analysis

---

## 📊 Core Metrics

### Outstanding Balance

```sql
Outstanding Balance = Remaining Loan Balance
```

---

### Interest Income

```sql
Interest Income = Σ(Interest Payment)
```

---

### Loan Yield

```sql
Loan Yield = Interest Income / Average Outstanding Balance
```

---

### NPL Ratio

```sql
NPL Ratio = Non-Performing Loans / Total Outstanding Loans
```

---

## 💡 Key Insights

### 1. Long-term loans accounted for a large proportion of the portfolio

Higher interest income potential was accompanied by increased duration and credit risk exposure.

---

### 2. Interest income increased steadily over time

Portfolio profitability remained highly dependent on outstanding loan growth.

---

### 3. Interest cashflow was front-loaded

Profitability was sensitive to prepayment behavior and loan repayment trends.

---

### 4. NPL ratio showed concentration in several customer segments

This indicated higher credit risk exposure within parts of the portfolio.

---

### 5. Scenario analysis improved visibility into portfolio sensitivity

Changes in prepayment and default assumptions significantly affected portfolio profitability and cashflow trends.

---

## 🚀 Business Impact

- Improved visibility into lending portfolio performance and cashflow trends
- Supported monitoring of credit risk indicators and portfolio quality
- Enabled analysis of profitability versus risk exposure
- Supported lending portfolio monitoring through interactive dashboard analytics

---

## 🔍 Future Enhancements

- Develop PD / LGD models for default prediction
- Analyze customer repayment and prepayment behavior
- Forecast:
  - Cashflow
  - Interest Income
  - NPL Trends
- Build stress-testing scenarios for:
  - Interest rate changes
  - Portfolio growth
  - Credit deterioration

---

## 🧩 Technology Stack

### SQL Server

- Stored Procedure
- CTE
- Window Function
- Aggregation

### Power BI

- Data Modeling
- DAX
- Visualization
- Risk Dashboard

---

## ✅ Key Takeaway

The project demonstrates how loan cashflow modeling and portfolio monitoring can support lending performance analysis and credit risk monitoring through SQL-based processing and Power BI analytics.

---

## 👩‍💻 Author

**Trang Thai**

GitHub: https://github.com/Trangthai-data
