# Revenue Cycle Analytics (MySQL)

## Overview
This project models and analyzes a healthcare revenue cycle using a relational MySQL database. 
The goal is to identify payor performance issues related to claim denials, cash collection efficiency,
and payment delays.

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

## Results Summary
- Cigna and Medi-Cal show the highest denial rates
- Self-Pay and Medicare demonstrate the highest collection efficiency
- Medi-Cal exhibits the longest average payment lag

## Next Steps
- Dashboarding in Tableau
- Trend analysis by service line and facility

