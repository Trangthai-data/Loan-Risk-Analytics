# 💳 Loan Cashflow & Credit Risk Analytics

![Dashboard](images/DASHBOARD%20LOAN.png)

Banking analytics project focusing on **loan cashflow analysis**, **credit risk monitoring**, and **lending portfolio optimization** from a banking perspective.

This project simulates how banks monitor loan performance, evaluate portfolio quality, and balance profitability with credit risk through cashflow modeling and scenario analysis.

---

## 🧠 Business Problem

Banks need to answer several critical questions:

- How do loans generate **cashflow and profitability** over time?
- Which customer segments contain the highest **credit risk**?
- How do **prepayment** and **default** impact interest income?

👉 The project focuses on balancing:

- Growth
- Yield
- Credit Risk

rather than only reporting loan balances.

---

## ⚠️ Challenges

- Loan cashflow data is fragmented across individual loan contracts
- Difficult to simultaneously monitor:
  - Principal
  - Interest
  - Outstanding Balance
- Lack of tools for evaluating:
  - Dynamic credit risk
  - Portfolio quality over time

---

## 🎯 Objectives

- Model loan cashflow (amortization)
- Calculate interest income over time
- Monitor outstanding balance
- Evaluate credit risk:
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
Stored Procedure (cashflow + outstanding)
        ↓
SQL View (data modeling)
        ↓
Power BI Dashboard (visualization & risk analysis)
```

---

## ⚙️ Technical Highlights

### SQL Development

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

---

### Data Modeling

#### Star Schema

- Date
- Customer
- Loan
- Fact Payment

---

### Power BI Features

- Data Modeling
- Risk Monitoring Dashboard
- Lending Portfolio Visualization
- Scenario Analysis

---

## 📊 Core Metrics

### Outstanding Balance

```text
Outstanding Balance = Remaining Loan Balance
```

---

### Interest Income

```text
Interest Income = Σ(Interest Payment)
```

---

### Loan Yield

```text
Loan Yield = Interest Income / Average Outstanding Balance
```

---

### NPL Ratio

```text
NPL Ratio = Non-Performing Loans / Total Outstanding Loans
```

---

## 💡 Insights & Decisions

### 1. Loan portfolio is concentrated in long-term tenor (~68%)

👉 Higher interest income potential but increased:
- Duration risk
- Credit concentration risk

---

### 2. Interest income grows steadily over time

👉 The portfolio is expanding well, but profitability heavily depends on outstanding loan growth.

---

### 3. Interest cashflow is front-loaded

👉 Profitability is highly sensitive to:
- Prepayment
- Customer churn

---

### 4. NPL ratio is extremely high (~90%) ⚠️

👉 This indicates:
- Serious credit quality issues
OR
- Risk classification logic may require recalibration

👉 Segmentation and risk classification should be reviewed carefully.

---

### 5. Coverage ratio remains very low (~2%)

👉 Provision buffers may not be sufficient to absorb future credit losses.

---

## 🚀 Business Impact

### 📉 Reduce concentration risk

- Rebalance long-term loan exposure
- Improve portfolio diversification

---

### 💰 Optimize risk-adjusted return

- Adjust loan pricing based on risk segments

---

### ⚠️ Improve NPL control

- Strengthen:
  - Monitoring
  - Early warning systems
  - Collection strategy

---

### 🛡️ Improve portfolio resilience

- Increase provisioning
- Improve coverage ratio

---

### 📊 Better credit decision-making

Support better trade-off analysis between:

- Growth
- Risk
- Yield

---

## 🔍 Future Enhancements

### Credit Risk Model

- Build PD / LGD models for default prediction

---

### Behavior Analysis

- Analyze:
  - Prepayment behavior
  - Customer repayment patterns

---

### Forecasting

- Forecast:
  - Cashflow
  - Interest Income
  - NPL

---

### Stress Testing

- Build what-if scenarios for:
  - Interest rate changes
  - Portfolio growth
  - Credit deterioration

---

### Portfolio Optimization

- Optimize risk-return tradeoff by:
  - Tenor
  - Customer segment

---

## 🧩 Technology Stack

### SQL

- CTE
- Window Function
- Aggregation
- Stored Procedure

---

### Power BI

- Data Modeling
- Visualization
- DAX
- Risk Dashboard

---

## ✅ Key Takeaway

The project demonstrates how banks can optimize lending profitability while balancing credit risk through loan cashflow analysis, portfolio monitoring, and scenario-based decision support.

---

## 👩‍💻 Author

**Trang Thai**

- GitHub: https://github.com/Trangthai-data
