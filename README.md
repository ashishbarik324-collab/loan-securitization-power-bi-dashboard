# Loan Securitisation & Risk Analysis Dashboard — Power BI

## 📊 Project Overview

This project is an interactive **Power BI dashboard for Loan Securitisation and Portfolio Risk Analysis**.

The dashboard analyzes loan portfolio performance across credit risk, defaults, collections, recoveries, vintage performance, borrower characteristics, and vehicle segments.

The objective of this project is to transform raw loan data into meaningful business insights that can support **portfolio monitoring, credit-risk assessment, collection analysis, and securitisation decision-making**.

---

## 🎯 Project Objectives

- Analyze overall loan portfolio performance
- Monitor loan defaults and delinquency
- Evaluate credit risk using CIBIL scores
- Analyze ECL and EAD exposure
- Track collections and recovery performance
- Analyze portfolio performance by vintage
- Identify trends in loan balances and payments
- Evaluate loan characteristics across different segments
- Analyze vehicle-wise loan performance and risk
- Build an interactive and management-friendly Power BI dashboard

---

## 🗂️ Dashboard Pages

The project contains **10 Power BI dashboard pages**:

### 1. Executive Overview
Provides a high-level summary of the loan portfolio using key performance indicators such as:
- Total Loans
- Current Pool Balance
- EAD
- ECL
- Default Rate
- Recovery Rate

### 2. Credit Risk Analysis
Analyzes:
- ECL exposure
- EAD exposure
- Default rate trends
- Recovery rate
- Delinquency status
- Loan distribution by delinquency

### 3. Portfolio & Performance Analysis
Analyzes:
- Current balance by vehicle type
- LTV and current balance
- Loan count trends
- Recovery amount
- EMI
- Total payments

### 4. Collection & Recovery Analysis
Focuses on:
- Recovery by loan purpose
- Recovery by region
- Delinquency status
- Payment trends
- Regional recovery performance

### 5. Vintage & Portfolio Trends Analysis
Analyzes:
- Cumulative defaults
- Cumulative default balance
- Cumulative recoveries
- Default rate by vintage
- Average current LTV
- Loan count by vintage

### 6. Collections & Recovery Trends
Analyzes recovery and collection trends over time:
- Collection efficiency
- Total recoveries
- Recovery rate
- Total payments
- Regional recovery amount
- Regional recovery rate

### 7. Vintage & Portfolio Trends
Provides additional vintage-level portfolio analysis including:
- Cumulative defaults
- Cumulative net loss
- Marginal loss rate
- Cumulative prepayments
- Average months on book
- Current 30+ day delinquency

### 8. Loan Performance & Risk
Analyzes loan performance using:
- CIBIL score at origination
- Current CIBIL score
- Current LTV
- Average current balance
- Recovery amount by CIBIL score
- Default rate by CIBIL score

### 9. Loan Characteristics & Delinquency
Analyzes loan characteristics by loan purpose:
- Default rate
- Interest rate
- Current LTV
- Original loan amount
- Original loan term
- Current balance

### 10. Vehicle-wise Loan Performance & Risk
Analyzes loan performance across vehicle types:
- Default rate
- Current LTV
- Interest rate
- Original loan amount
- Original loan term
- Current balance

---

## 🛠️ Tools & Technologies

- **Power BI**
- **DAX**
- **Microsoft Excel**
- **Data Modelling**
- **Data Visualization**
- **Power Query**

---

## 📐 Data Model

The Power BI model consists of multiple tables used for portfolio analysis:

- `Loan`
- `History`
- `Monthly_Performance`
- `Vintage`
- `Calendar`
- `Measures`

A dedicated **Measures** table is used to organize DAX calculations.

The model also uses a **Calendar table** for time-based analysis and relationships with relevant date fields.

---

## 📊 Key Metrics

Some of the major metrics calculated in the project include:

- Total Loans
- Defaulted Loans
- Default Rate
- Current Pool Balance
- EAD
- ECL
- Gross Loss
- Total Recoveries
- Recovery Rate
- Collection Efficiency
- Current LTV
- Cumulative Defaults
- Cumulative Recoveries
- Cumulative Net Loss

---

## 🧮 DAX

DAX was used to create calculated measures for portfolio and risk analysis.

Example:

```DAX
Default Rate =
DIVIDE(
    [Defaulted Loans],
    [Total Loans],
    0
)
