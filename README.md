\# Procurement \& Supply Chain Analysis — DataCo Global



\## Objective

Analyzed real order-line data from a global manufacturing/retail supply chain to

identify procurement consolidation opportunities and category-level

standardization candidates, a methodology directly relevant to industrial

inventory/procurement problems (e.g. spares consolidation, working capital

reduction).



\## Data Source

[\[DataCo Smart Supply Chain for Big Data Analysis]](https://www.kaggle.com/datasets/shashwatwork/dataco-smart-supply-chain-for-big-data-analysis)

(Kaggle, uploaded by shashwatwork) 

It is a real transactional data from DataCo Global,

\~180,000 order-line records across 50+ product categories and multiple regions.



\## Method

1\. Cleaned and validated \~180K order records in Excel (removed data errors,

&#x20;  added calculated Order Value field).

2\. Built a category-level summary via PivotTable: total order value, order

&#x20;  frequency, and average profit ratio per category.

3\. Classified each category into \*\*High-value / Low-frequency / Stable\*\*

&#x20;  using data-driven percentile thresholds (75th percentile of order value,

&#x20;  25th percentile of order frequency) rather than arbitrary cutoffs.

4\. Built a Pareto (cumulative %) analysis to quantify value concentration.

5\. Built an interactive Power BI dashboard to visualize findings.



\## Key Findings

\- \*\*\~18% of categories (9 of 50) account for over 80% of total order value\*\* —

&#x20; a small set of core categories (Fishing, Cleats, Camping \& Hiking, Cardio

&#x20; Equipment, Women's Apparel, Water Sports, Men's Footwear, Indoor/Outdoor

&#x20; Games, Shop By Sport) drives the majority of order value — a classic

&#x20; Pareto/ABC pattern.

\- \*\*13 categories flagged "High-value," collectively \~93% of total order

&#x20; value\*\* — recommend prioritizing supplier standardization/consolidation

&#x20; review here first, since this is where the greatest financial leverage sits.

\- \*\*13 categories flagged "Low-frequency"\*\* (Sporting Goods, Health and

&#x20; Beauty, Strength Training, Men's Golf Clubs, Women's Golf Clubs, Men's

&#x20; Clothing, and others) — candidates for consolidated or less frequent

&#x20; procurement cycles to reduce overhead, mirroring real spares/procurement

&#x20; consolidation logic. Notably, the categories split into three roughly

&#x20; equal groups — 13 High-value, 13 Low-frequency, and \~24 Stable — making

&#x20; the "focus vs. deprioritize" distinction clear and actionable.

\- Cross-referencing value against order frequency (scatter analysis) shows

&#x20; most categories cluster near the origin (low value, low frequency), while

&#x20; a handful of outliers — e.g. \*\*Fishing\*\*, which combines the highest total

&#x20; order value with comparatively modest order frequency — warrant individual

&#x20; review rather than blanket treatment by flag alone.



\## Assumptions \& Limitations

\- This is order-line transaction data, not warehouse stock-level data —

&#x20; "inventory movement" here is inferred from order value and frequency, a

&#x20; standard demand-based proxy when real stock-on-hand data isn't available.

\- Percentile thresholds (75th/25th) were chosen for a reasonably selective

&#x20; "High-value"/"Low-frequency" split; different thresholds would shift

&#x20; category counts but not the underlying Pareto pattern.



\## Dashboard

!\[dashboard](screenshots/dashboard.png)



\## Tools

Excel, Power BI Desktop, Git/GitHub.

