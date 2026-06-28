# Part 4: Tableau Executive Dashboard & Data Storytelling

## Business Problem
The leadership team of a retail chain needed an executive dashboard to monitor sales performance, profitability, category performance, shipping efficiency, discount impact, and return patterns across regions and customer segments.


## Dataset
**File:** dashboard_sales_data.xlsx  
**Records:** 4,200 orders  
**Columns:** 20 — order_id, order_date, ship_date, customer_id, customer_segment, region, state, city, category, sub_category, product_name, ship_mode, sales, quantity, discount, profit, return_flag, delivery_days, customer_rating, campaign_channel  
**Missing values:** customer_rating (32 rows), campaign_channel (24 rows)


## Tableau Workbook
**File:** tableau/executive_dashboard.twbx  
The workbook contains 7 individual views and 1 executive dashboard combining all key charts with interactive filters.


## Calculated Fields Created

| Field | Formula |
|---|---|
| Profit Margin | PROFIT / SALES |
| Cost | SALES - PROFIT |
| Average Order Value | SUM(Sales) / COUNTD(Order ID) |
| Return Rate | SUM(Return Flag) / COUNT(Order ID) |
| Shipping Delay Bucket | IF delivery_days ≤ 1 THEN "Fast" ELSEIF ≤ 3 THEN "Standard" ELSE "Delayed" END |


## Dashboard Components

| View | Chart Type | Purpose |
|---|---|---|
| Sales Trend | Line chart | Monthly sales over time |
| Regional Performance | Bar chart | Sales and profit by region |
| Category Profitability | Treemap | Category/sub-category profit and margin |
| Customer Segment | Bar chart | Segment comparison |
| Discount vs Profit | Scatter plot | Discount-profit relationship |
| Shipping Performance | Bar chart | Delivery days by ship mode |
| Return Analysis | Highlight table | Return rate by category and segment |


## Filters and Interactions
- Region filter (applies to all sheets)
- Category filter (applies to all sheets)
- Customer Segment filter
- Date range filter (Order Date)
- Ship Mode filter
- Dashboard action: clicking a region on the map highlights all other charts for that region


## Key Business Insights
- Technology drives ~85% of total profit despite being 1 of 3 categories
- South region leads in sales volume (₹6.47 Cr)
- Orders with negative profit have average discount of 27.3% vs 12.7% for profitable orders
- Furniture return rate (7.67%) is more than double Technology (3.03%)
- Standard Class shipping averages 4.71 days — the most common mode and the slowest
- All customer segments have consistent profit margins (~15%) — volume is the key differentiator

---
