# **Procurement \& Supply Chain Analysis — DataCo Global**



## Objective

Analyzed real order-line data from a global manufacturing/retail supply chain to identify procurement consolidation opportunities and category-level standardization candidates, a methodology directly relevant to industrial inventory/procurement problems.

## 

## Data Source

\[\[DataCo Smart Supply Chain for Big Data Analysis]](https://www.kaggle.com/datasets/shashwatwork/dataco-smart-supply-chain-for-big-data-analysis)

(Kaggle, uploaded by shashwatwork)

It is a real transactional data from DataCo Global,

\~180,000 order-line records across 50+ product categories and multiple regions.



## Method

1\. Cleaned and validated \~180K order records in Excel (removed data errors, added calculated Order Value field).

2\. Built a category-level summary via PivotTable: total order value, order frequency, and average profit ratio per category.

3\. Classified each category into \*\*High-value / Low-frequency / Stable using data-driven percentile thresholds (75th percentile of order value, 25th percentile of order frequency) rather than arbitrary cutoffs.

4\. Built a Pareto (cumulative %) analysis to quantify value concentration.

5\. Built an interactive Power BI dashboard to visualize findings.



## Key Findings

(i) ***\~18% of categories (9 of 50)*** account (for over 80% of total order value) a small set of core categories (Fishing, Cleats, Camping \& Hiking, Cardio Equipment, Women's Apparel, Water Sports, Men's Footwear, Indoor/Outdoor Games, Shop By Sport) drives the majority of order value a classic Pareto pattern.

(ii) ***13 categories flagged "High-value,"*** collectively (\~93% of total order value) — recommend prioritizing supplier standardization/consolidation review here first, since this is where the greatest financial leverage sits.

(iii) ***13 categories flagged "Low-frequency"*** (Sporting Goods, Health and Beauty, Strength Training, Men's Golf Clubs, Women's Golf Clubs, Men's Clothing, and others) — candidates for consolidated or less frequent procurement cycles to reduce overhead, mirroring real spares/procurement consolidation logic. Notably, the categories split into three roughlyequal groups — 13 High-value, 13 Low-frequency, and \~24 Stable — making the "focus vs. deprioritize" distinction clear and actionable.

(iv) Cross-referencing value against order frequency (scatter analysis) shows most categories cluster near the origin (low value, low frequency), while a handful of outliers. Example - Fishing, which combines the highest total order value with comparatively modest order frequency — warrant individual review rather than blanket treatment by flag alone.



## Assumptions \& Limitations

\- This is order-line transaction data, not warehouse stock-level data; "inventory movement" here is inferred from order value and frequency, a standard demand-based proxy when real stock-on-hand data isn't available.

\- Percentile thresholds (75th/25th) were chosen for a reasonably selective "High-value"/"Low-frequency" split; different thresholds would shift category counts but not the underlying Pareto pattern.



## Dashboard

!\[dashboard](screenshots/dashboard.png)



## Tools

Kaggle, 
Excel, Power BI Desktop, GitHub.

