# Chart Selection Justification
**Name:** Radha Manasa Peesapati | **Date:** 28 June 2026

---

## Sales Trend — Line Chart
**Purpose:** Show how sales change month by month across regions.  
**Why line chart:** Standard for time-series data. Shows direction and rate of change clearly.  
**Fields:** Order Date (month) on X-axis, SUM(Sales) on Y-axis, Region on Color.  
**Design principle:** Minimal gridlines, no markers — keeps focus on the trend.  
**Mistake avoided:** Bar chart for time series compresses the trend and makes patterns harder to read.

---

## Regional Performance — Horizontal Bar Chart
**Purpose:** Compare total sales and profit across regions.  
**Why horizontal bars:** Good for comparing discrete categories. Horizontal layout makes labels readable without rotation.  
**Fields:** Region on Rows, SUM(Sales) and SUM(Profit) on Columns, Region on Color.  
**Design principle:** Sorted by sales descending — highest region visible immediately.  
**Mistake avoided:** Pie chart would hide the magnitude of differences between regions.

---

## Category Profitability — Bar Chart with Colour
**Purpose:** Show profit by category and sub-category with margin visible through colour.  
**Why bar chart with colour encoding:** Bars show absolute profit. Colour (Profit Margin) adds a second dimension without adding clutter.  
**Fields:** Category and Sub Category on Rows, Profit on Columns, Profit Margin on Color.  
**Design principle:** Two dimensions in one view — size for profit, colour for margin.  
**Mistake avoided:** Two separate charts would require the reader to mentally combine them.

---

## Customer Segment — Side-by-Side Bar Chart
**Purpose:** Compare Sales and Profit across three customer segments.  
**Why side-by-side bars:** Three segments with two metrics — easy to compare both within and across segments.  
**Fields:** Customer Segment on Rows, Sales and Profit on Columns, Segment on Color.  
**Design principle:** Consistent colour per segment across the dashboard.  
**Mistake avoided:** Stacked bars make it harder to read individual segment values accurately.

---

## Discount vs Profit — Scatter Plot
**Purpose:** Show the relationship between discount level and profit at order level.  
**Why scatter plot:** Best chart type for showing correlation between two continuous variables across many records.  
**Fields:** Discount on X-axis, Profit on Y-axis, Category on Color. Aggregate Measures turned off.  
**Design principle:** Reference lines at average discount and average profit divide the chart into quadrants.  
**Mistake avoided:** Using averages only (bar chart) would hide the spread and the loss-making outliers.

---

## Shipping Performance — Horizontal Bar Chart
**Purpose:** Show average delivery days by shipping mode.  
**Why bar chart:** Four categories with one metric — simple comparison. Horizontal layout for label readability.  
**Fields:** Ship Mode on Rows, AVG(Delivery Days) on Columns, Shipping Delay Bucket on Color.  
**Design principle:** Sorted fastest to slowest — Same Day at top, Standard Class at bottom.  
**Mistake avoided:** Line chart would imply a continuous relationship between shipping modes which doesn't exist.

---

## Return Analysis — Highlight Table
**Purpose:** Show return rate across category and customer segment combinations.  
**Why highlight table:** Shows two dimensions (category × segment) in one grid with colour encoding the return rate.  
**Fields:** Category on Columns, Customer Segment on Rows, AVG(Return Flag) on Color.  
**Design principle:** Single-colour scale — darker means higher return rate. Easy to spot high-risk combinations.  
**Mistake avoided:** Multiple bar charts would take more space and make cross-dimensional comparison harder.
