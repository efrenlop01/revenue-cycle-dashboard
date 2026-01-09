# Revenue Cycle Analytics (MySQL)

## Overview
This project models and analyzes a healthcare revenue cycle using a relational MySQL database. 
The goal is to identify payor performance issues related to claim denials, cash collection efficiency,
and payment delays.

## Business Questions Addressed
- Which payors contribute the highest claim denial rates?
- Where is revenue leakage occurring due to low collection efficiency?
- How long does it take to receive payment after claim submission?
- Which payors and service lines create the most AR lag?

## Data Model
- patients
- encounters
- claims
- payments

Primary and foreign keys enforce referential integrity across the revenue cycle.

## Key Metrics
- Denial Rate by Payor
- Collection Rate (Paid vs Billed)
- Average Days to Payment (A/R Proxy)

## Tools Used
- MySQL 8.0
- MySQL Workbench
- SQL (joins, aggregations, CASE statements)

 ## SQL Highlights
- Multi-table joins across claims, encounters, and payments
- Aggregations using GROUP BY (payor, service line, month)
- CASE statements to flag denied claims
- Date calculations to compute average days to payment
- Creation of derived KPI tables for downstream analysis


## Results Summary
- Cigna and Medi-Cal show the highest denial rates
- Self-Pay and Medicare demonstrate the highest collection efficiency
- Medi-Cal exhibits the longest average payment lag

## Business Impact Interpretation

- High denial rates for Cigna and Medi-Cal may indicate authorization or eligibility issues.
- Self-Pay and Medicare demonstrate stronger collection efficiency, suggesting lower write-offs.
- Longer payment lags for Medi-Cal may negatively impact cash flow and AR aging.

