# Business Insights
**Name:** Radha Manasa Peesapati | **Date:** June 2026

---

## Calculated Fields Created

| Field | Formula |
|---|---|
| Profit Margin | SUM([Profit]) / SUM([Sales]) |
| Cost | SUM([Sales]) - SUM([Profit]) |
| Avg Order Value | SUM([Sales]) / COUNTD([Order Id]) |
| Return Rate | SUM([Return Flag]) / COUNT([Order Id]) |
| Shipping Delay Bucket | IF delivery_days ≤ 1 THEN "Fast" ELSEIF ≤ 3 THEN "Standard" ELSE "Delayed" END |

---

## Insight 1 — Sales Trend
South region consistently leads in monthly sales throughout the year, peaking around October-November. The other three regions are relatively close to each other. No major dips were observed across any region which suggests stable demand.

**Recommended action:** Investigate what drives South's consistent lead — could be campaign mix, product mix, or regional demand — and replicate in East and West.

---

## Insight 2 — Regional Performance
South generates the highest total sales (₹6.47 Cr) and profit (₹10M+). East has the lowest sales but its profit is comparable to West. All regions have similar profit margins (~15%) which means the difference is in volume, not efficiency.

**Recommended action:** Focus on volume-driving strategies in East rather than margin improvement.

---

## Insight 3 — Category Profitability
Technology accounts for almost all the profit — Copiers, Phones, and Accessories are the top three sub-categories by a wide margin. Furniture sub-categories are a distant second. Office Supplies contribute very little despite likely high order volumes.

**Recommended action:** Prioritise Technology in marketing budgets. Review Office Supplies pricing to improve contribution.

---

## Insight 4 — Customer Segment Behaviour
Home Office leads in both sales and profit, slightly ahead of Consumer and Corporate. All three segments have very similar profit margins (~15%). The difference between segments is mostly in volume.

**Recommended action:** Target Home Office segment for upselling since they already show the highest spend.

---

## Insight 5 — Discount Impact
Orders with negative profit have an average discount of 27.3% compared to 12.7% for profitable orders. The scatter plot clearly shows profit declining as discounts increase, especially for Furniture.

**Recommended action:** Set a hard cap at 20% discount. Orders above 25% should require approval — they are likely loss-making.

---

## Insight 6 — Shipping Performance
Same Day delivers in under 1 day on average. Standard Class averages 4.71 days — the most commonly used but slowest mode. First Class at 1.77 days is a good middle ground.

**Recommended action:** Promote First Class as a value-speed option. Review whether Standard Class SLA is affecting customer satisfaction scores.

---

## Insight 7 — Return Pattern
Furniture has a 7.67% return rate — more than double Technology (3.03%) and Office Supplies (3.65%). Within Furniture, the Home Office segment shows the highest return rate.

**Recommended action:** Investigate top returned Furniture products. Review product descriptions and packaging to reduce damage-related returns.

---

## Insight 8 — Business Risk
A small number of deeply discounted large orders generate losses of up to ₹17,757 per order. These are concentrated in Furniture and appear across all regions. Without a discount policy, a few bad orders can significantly dent monthly profitability.

**Recommended action:** Introduce a pre-approval workflow for discounts above 20%. The financial risk per order is high enough to justify the process overhead.
