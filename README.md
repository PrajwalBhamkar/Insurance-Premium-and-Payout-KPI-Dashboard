# 🧾 Insurance Premium and Payout KPI Dashboard

*A comprehensive, interactive Power BI dashboard developed for True Secure Credit Insurance to analyze the insurance policy lifecycle, financial performance amounts from 2015 to 2025.*

---

## 📌 Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Tools & Technologies](#tools--technologies)
- [Methods](#methods)
- [Key Insights](#key-insights)
- [Dashboard / Model / Output](#dashboard--model--output)
- [Results & Conclusion](#results--conclusion)
- [Author & Contact](#author--contact)

---

## Overview

This project was initiated for **True Secure Credit Insurance**, a financial company in India offering protection plans for individuals and businesses. The goal was to create a unified, interactive analytics solution using **Microsoft Power BI**, covering the insurance policy lifecycle from **2015 to 2025**.

The dashboard provides insights into:

- Policy performance
- Maturity forecasting
- Customer segmentation
- Geographic and product performance

---

## Problem Statement

The objective was to build an **interactive dashboard** analyzing insurance policy data and delivering actionable insights.

### 🎯 Key Business Goals

- **Performance Tracking:** Analyze policy performance across segments.
- **Geographic & Product Analysis:** Identify strong vs. weak regions/policy types.
- **Product Uptake:** Detect top and low-performing plans.
- **Team Accountability:** Track performance of sales and servicing teams.

### 🚫 Client Constraint

Focus **only** on policies with **Active** status.
Claims and loan-related data must be **excluded**.

---

## Dataset

Data covering the policy lifecycle from **2015–2025** was provided as multiple CSV files and structured into a **Star Schema**.

### **Data Model Overview**

| Table Type           | Key Tables                                                                                             |
| -------------------- | ------------------------------------------------------------------------------------------------------ |
| **Fact Table**       | Insurance Policy Fact (Policy Number, Status, Start Date, Premium Amount, Tenure, IDs)                 |
| **Dimension Tables** | Customer Detail, Insurance Agent, Policy Protection Plan, Policy Type, Regional Manager, Zonal Manager |

---

## Tools & Technologies

- **Dashboarding:** Microsoft Power BI
- **Data Transformation:** Excel,Power Query Editor
- **Calculations:** DAX (Data Analysis Expressions)

---

## Methods

### 1. Data Architecture & Modeling 📐

- CSV ingestion into Power Query Editor
- Cleaning steps: remove blanks, fix data types, standardize numeric fields
- **Star Schema** implemented
- Relationships formed using PK–FK keys
- Bi-directional cross-filtering enabled

### 2. KPI & DAX Calculations 🧮

Key formulas include:

- **Total Annual Premium** – normalized premium frequency
- **Total Premium Amount** – annual premium × tenure
- **Premium Payment Duration** – DATEDIFF logic
- **Total Premium Paid / Payable**
- **Maturity Amount** using VAR blocks & rate matrix logic
- **Annualized ROI (%), CAGR (%)** using POWER, DIVIDE, and error handling
- **Payment & Maturity Buckets** for forecasting

---

## Key Insights

- **Endowment** policy type leads with **34.89%** of Total Annual Premium.
- **ULIP Growth Plan** contributes **32.74%** of Total Premium paid.
- Average **Annualized ROI ≈ 8.87%**.
- Average **annual fixed growth rate ≈ 9.50%**.
- Out of the **39,096.58 million** total premium amount:
  - **33.17%** (10,686.35M) is paid
  - **66.83%** (28,410.24M) is payable
- **Sum Assured** typically ranges **3–4×** the annual premium.
- Payment Buckets forecast future maturity/premium timelines.

---

## Dashboard / Model / Output

The dashboard contains **five pages**:

1. **Summary Page**
   - KPIs: Active Policies (7,299), Total Premium Amount (39.09B), Total Annual Premium (2.16B), Underwriting Expense (38.66M)
   - Detailed policy table

2. **Insurance Overview**
   - Pie, Donut, Tree Map, Bar, and Area charts
   - Dynamic measures via Field Parameters

3. **Investment vs. Maturity Value**
   - Line + clustered column chart comparing investment vs. maturity

4. **Premium Analysis**
   - Premium paid vs payable
   - Payment Buckets for forecasting

---


## Results & Conclusion

The **Insurance Premium and Payout KPI Dashboard** provides:

📈 **Unified insights** into policy performance, maturity forecasting, premium trends, and investment growth.

⚙️ **Automation & efficiency** through optimized DAX measures, dynamic visuals, and an intuitive multi-page reporting structure.

📊 **Accurate forecasting tools** using Payment Buckets and Maturity calculations to help the organization plan future cash flows and understand long-term liabilities.

This dashboard enables True Secure Credit Insurance to make **data-driven decisions**, identify high-value policy plans, analyze premium payment behaviours, and strategically plan for future payouts and premium growth.

---

## Author & Contact

**Prajwal Bhamkar**
📧 Email: bhamkarprajwal8@gmail.com


---

## 📊 Dashboard Overview
https://github.com/PrajwalBhamkar/Insurance-Premium-and-Payout-KPI-Dashboard/blob/main/Dashboard-snapshot.png
