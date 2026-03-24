# superstore-profitability-dashboard
Analyzed a $2.3M retail portfolio (~10K orders) to identify profit leakage drivers, uncovering margin erosion in key sub-categories and enabling targeted pricing strategy recommendations.
## Overview
This project identifies profit leakage drivers in a $2.3M retail portfolio by analyzing the impact of discounting, product mix, and sub-category performance.

Key finding: Profitability erosion is concentrated in specific sub-categories (Tables, Bookcases, Supplies) driven by excessive discounting, while other categories remain resilient even at higher discount levels.

## Business Problem
Revenue alone does not explain business performance. A company may generate strong sales while still underperforming on profit due to weak margins, excessive discounting, or poor product mix.

This dashboard was built to answer:
- Which categories and sub-categories are driving or hurting profitability?
- How does discounting affect profit?
- Are losses broad-based or concentrated in specific areas?
- What actions could improve pricing and margin performance?

## Tools Used
- Power BI
- SQL
- PostgreSQL
- Excel / CSV

## Dataset
- Sample Superstore dataset
- ~9,994 orders
- Fields used include Sales, Profit, Discount, Category, Sub-Category, Region, and Order Date

## Dashboard Features
- KPI summary: Total Sales, Total Profit, Total Orders, Profit Margin
- Category profit contribution
- Regional sales contribution
- Discount vs profit analysis
- Sub-category profit contribution
- Sub-category profit margin analysis
- Key business insights panel

## Key Insights
- Profitability is highly concentrated — losses are driven by a few sub-categories, not the entire portfolio
- Tables and Bookcases are structurally unprofitable, indicating pricing or cost issues
- Discounting has a nonlinear impact — some categories remain profitable at higher discounts while others quickly erode margin
- A uniform discount strategy leads to margin leakage and inefficient pricing decisions

## Business Recommendations
- Eliminate or significantly reduce discounting on loss-making sub-categories (Tables, Bookcases)
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


## What I Learned
This project reinforced the importance of analyzing profitability at a more granular level rather than relying on top-line revenue. It also showed how pricing and discount strategies can have uneven effects across categories, making segmented decision-making more effective than a one-size-fits-all approach. This analysis highlights the importance of moving beyond aggregated metrics and evaluating profitability at the sub-category level to uncover hidden performance drivers.

## Next Steps
- Add customer segment analysis
- Add time trend analysis for profit and discounting
- Build a second version using Power BI Desktop with richer modeling
- Expand the project into a pricing simulation or scenario analysis dashboard
