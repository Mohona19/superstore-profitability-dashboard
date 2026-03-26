# Superstore Pricing Optimization & Profitability Analysis

Analyzed a $2.3M retail portfolio (~10K orders) to identify profit leakage drivers, uncovering margin erosion in key sub-categories and enabling targeted pricing strategy recommendations.

This project evolved from a profitability dashboard into a pricing optimization simulation. A rule-based pricing strategy was applied to adjust discount levels based on product-level profitability, and the potential impact was measured.

## Key Result
- Estimated profit increase: **+34% (~$97K)**
- Primary uplift driver: reduced discounting in loss-making sub-categories such as **Tables** and **Bookcases**

## Business Problem
Revenue alone does not explain business performance. A company may generate strong sales while still underperforming on profit due to weak margins, excessive discounting, or poor product mix.

This project was built to answer:
- Which categories and sub-categories are driving or hurting profitability?
- How does discounting affect profit?
- Are losses broad-based or concentrated in specific areas?
- What actions could improve pricing and margin performance?

## Project Evolution
This project was completed in two stages:

### 1. Profitability Analysis Dashboard
Built an interactive Power BI dashboard to diagnose margin leakage across categories, sub-categories, and regions.

### 2. Pricing Optimization Simulation
Extended the analysis into a simulation model that applied rule-based discount adjustments and estimated the resulting profit uplift.

## Tools Used
- Power BI
- SQL
- PostgreSQL
- Excel / CSV

## Dataset
- Sample Superstore dataset
- ~9,994 orders
- Fields used: Sales, Profit, Discount, Category, Sub-Category, Region, and Order Date

## Dashboard Features
- KPI summary: Total Sales, Total Profit, Total Orders, Profit Margin
- Category profit contribution
- Regional sales contribution
- Discount vs profit analysis
- Sub-category profit contribution
- Sub-category profit margin analysis
- Pricing optimization simulation
- Key business insights panel

## Key Insights
- Profitability is highly concentrated — losses are driven by a few sub-categories, not the entire portfolio
- Tables and Bookcases are structurally unprofitable, indicating pricing or cost issues
- Discounting has a nonlinear impact — some categories remain profitable at higher discounts while others quickly erode margin
- A uniform discount strategy leads to margin leakage and inefficient pricing decisions

## Business Recommendations
- Eliminate or significantly reduce discounting on loss-making sub-categories such as Tables and Bookcases
- Implement margin-based discount thresholds instead of uniform discounting
- Prioritize sales efforts toward high-margin categories such as Technology and Copiers
- Conduct pricing and cost diagnostics for persistently unprofitable products

## SQL Analysis
Sample SQL questions used in the analysis included:
- Profit by category
- Profit by sub-category
- Profit margin by sub-category
- Discount vs average profit
- Regional sales contribution


See [`sql/profitability_analysis.sql`](sql/profitability_analysis.sql)

## Screenshots
### Dashboard Overview
<img width="804" height="682" alt="Dashboard Overview" src="https://github.com/user-attachments/assets/c5786429-bb1e-46c6-a5b2-825f6312d45b" />


### Profit by Sub-Category
<img width="245" height="273" alt="Profit by subcategory" src="https://github.com/user-attachments/assets/20deb1c9-19ad-4480-a586-06b29b9cf192" />


### Discount vs Profit
<img width="255" height="202" alt="Discount vs Profit" src="https://github.com/user-attachments/assets/65a0847c-878c-491f-9eff-f8fafa260e58" />

**Pricing Optimization Simulation**
<img width="778" height="659" alt="dashboard_overview" src="https://github.com/user-attachments/assets/cc407259-2abd-4c1a-8cf6-6b827674f63e" />

**pricing_optimization_KPI_view**
<img width="635" height="77" alt="pricing_optimization_view" src="https://github.com/user-attachments/assets/4bee8999-be31-4dfa-8f2f-83e3f38049a6" />

## What I Learned
This project reinforced the importance of analyzing profitability at a granular level rather than relying only on top-line revenue. It also showed that pricing and discount strategies affect categories differently, making segmented decision-making more effective than a one-size-fits-all approach. Evaluating performance at the sub-category level helped uncover hidden margin leakage that would have been missed in aggregate reporting.

## Next Steps
- Add customer segment analysis
- Add time trend analysis for profit and discounting
- Rebuild the model in Power BI Desktop for richer scenario modeling
- Extend the simulation with Python-based predictive modeling
Final notes

## What I Learned
This project reinforced the importance of analyzing profitability at a granular level rather than relying only on top-line revenue. It also showed that pricing and discount strategies affect categories differently, making segmented decision-making more effective than a one-size-fits-all approach. Evaluating performance at the sub-category level helped uncover hidden margin leakage that would have been missed in aggregate reporting.

## Next Steps
- Add customer segment analysis
- Add time trend analysis for profit and discounting
- Rebuild the model in Power BI Desktop for richer scenario modeling
- Extend the simulation with Python-based predictive modeling

## What I Learned
This project reinforced the importance of analyzing profitability at a granular level rather than relying only on top-line revenue. It also showed that pricing and discount strategies affect categories differently, making segmented decision-making more effective than a one-size-fits-all approach. Evaluating performance at the sub-category level helped uncover hidden margin leakage that would have been missed in aggregate reporting.

## Next Steps
- Add customer segment analysis
- Add time trend analysis for profit and discounting
- Rebuild the model in Power BI Desktop for richer scenario modeling
- Extend the simulation with Python-based predictive modeling
