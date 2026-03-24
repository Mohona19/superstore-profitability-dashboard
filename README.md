# superstore-profitability-dashboard
## Overview
This project analyzes sales, profit, discount behavior, and sub-category performance using the Superstore dataset. The goal was to move beyond surface-level revenue reporting and identify what was driving profitability leakage across the portfolio.

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
- Furniture was the weakest category by profit contribution
- Tables, Bookcases, and Supplies had negative profit margins
- Profit leakage was concentrated, not uniform across the portfolio
- Higher discounts were often associated with lower profitability
- Some sub-categories remained profitable despite higher discounts, suggesting discount sensitivity differs by product group
- A uniform discount strategy is inefficient and should be replaced with more segmented pricing decisions

## Business Recommendations
- Reduce or cap discounts for structurally weak sub-categories such as Tables and Bookcases
- Reassess pricing and cost structure for consistently unprofitable products
- Apply discounting more selectively based on product-level margin sensitivity
- Focus commercial effort on high-margin categories and sub-categories

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
screenshots/Dashboard Overview.png

### Profit by Sub-Category
![Profit by Sub-Category](screenshots/profit-by-subcategory.png)

### Discount vs Profit
![Discount vs Profit](screenshots/discount-vs-profit.png)

## What I Learned
This project reinforced the importance of analyzing profitability at a more granular level rather than relying on top-line revenue. It also showed how pricing and discount strategies can have uneven effects across categories, making segmented decision-making more effective than a one-size-fits-all approach.

## Next Steps
- Add customer segment analysis
- Add time trend analysis for profit and discounting
- Build a second version using Power BI Desktop with richer modeling
- Expand the project into a pricing simulation or scenario analysis dashboard
