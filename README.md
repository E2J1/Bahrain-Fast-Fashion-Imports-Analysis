# Bahrain Fast Fashion Imports Analysis (2021–2025)

A market intelligence and business intelligence project analyzing Bahrain’s fast fashion import trends to support a data-driven market entry strategy for a new apparel retailer.

---

# Data Dictionary

| Column Name | Description |
| --- | --- |
| `year` | Year of the import record. |
| `month` | Month when the import transaction was recorded. |
| `commodity_no` | Commodity classification code used to identify the apparel product type. |
| `commodity` | Description of the imported clothing item. |
| `un_code` | Country code of the exporting/supplier country. |
| `country_name` | Name of the country exporting the apparel products to Bahrain. |
| `import_value_bd` | Import value measured in Bahraini Dinar (BD). |
| `import_value_usa` | Import value converted to US Dollars (USD). |
| `import_weight_kg` | Total imported weight measured in kilograms. |
| `import_quantity` | Number of imported units/items. |
| `um` | Unit of measurement used for the imported quantity, such as number of items (`NO`). |

---

## Dashboard Preview

![Dashboard Overview](images/dashboard-overview.png)

---

## Interactive Dashboard Demo

![Dashboard Demo](images/dashboard-demo.gif)

> Interactive Power BI dashboard featuring seasonal filters, sourcing analysis, KPI tracking, and clothing category insights.

---

# Project Overview

This project analyzes five years of Bahrain’s apparel import data to uncover:

- Market growth trends
- High-demand clothing categories
- Seasonal purchasing patterns
- Supplier country performance
- Cost-efficient sourcing opportunities

The goal was to transform raw trade data into actionable business insights for a fast fashion brand entering the Bahraini market.

---

# Business Problem

A new fast fashion retailer lacked visibility into:

- Which clothing categories dominate Bahrain’s import market
- Which countries provide the most cost-efficient sourcing
- When seasonal demand peaks occur
- Which product categories offer the highest commercial opportunity

This analysis provides a data-backed framework for inventory planning, sourcing strategy, and market positioning.

---

# Business Questions Answered

- Which apparel categories generate the highest import value?
- Which products dominate import volume?
- Which supplier countries provide the lowest average cost per item?
- How has Bahrain’s apparel market grown between 2021–2025?
- Which months and seasons experience peak demand?
- Which categories present premium market opportunities?

---

# Key Insights

## Market Growth Analysis

![Market Growth](images/market-growth.png)

- Bahrain’s apparel import value increased by approximately **41%** between 2021 and 2025
- Total import value peaked at **BD 87M** in 2024
- Growth remained consistent across multiple years, signaling sustained market demand

---

## Commodity Analysis

![Commodity Analysis](images/commodity-analysis.png)

### Highest Import Value Categories
- Trousers & Shorts — BD 96M
- Dresses — BD 74M
- T-shirts — BD 65M

### Key Findings
- T-shirts dominated import volume but operated on thinner margins
- Dresses showed strong premium positioning potential
- Trousers & Shorts represented the largest commercial opportunity

---

## Supplier Country Analysis

![Country Analysis](images/country-analysis.png)

### Key Findings
- China dominated total import value
- India and Bangladesh offered the lowest average cost per item (~BD 2)
- Italy operated as a premium-priced supplier market

### Business Implication
India and Bangladesh provide the strongest balance between:
- Low sourcing cost
- Shorter lead times
- High apparel manufacturing volume

---

## Seasonal Demand Insights

### Key Findings
- Demand peaks occurred during:
  - January–March
  - December
- Seasonal patterns remained relatively consistent across multiple years
- Winter and Summer represented the strongest inventory periods

### Business Implications
Retailers should align supplier ordering cycles during:
- October
- November

This helps ensure inventory arrives before peak seasonal demand periods and reduces the risk of stock shortages.

---

# Strategic Recommendations

![Strategic Recommendations](images/recommendations.png)

### Product Strategy
Focus on:
- T-shirts
- Trousers & Shorts
- Dresses

These categories consistently dominated Bahrain’s import market and represented the strongest commercial opportunity.

### Sourcing Strategy
- Source core inventory from India and Bangladesh
- Use China for high-variety trend-driven inventory
- Delay premium sourcing markets until brand positioning matures

### Inventory Timing
Align purchasing cycles around:
- Q1 demand peaks
- December seasonal demand

This helps optimize stock availability and reduce inventory shortages during high-demand periods.

---

# Tech Stack

## Data Analysis
- Python
- Pandas

## Data Visualization
- Power BI

## Data Processing
- Data Cleaning
- Data Transformation
- KPI Development
- Trend Analysis

---

# Repository Structure

```bash
.
├── data/
├── images/
│   ├── dashboard-overview.png
│   ├── dashboard-demo.gif
│   ├── market-growth.png
│   ├── commodity-analysis.png
│   └── country-analysis.png
├── notebooks/
│   ├── bahrain_imports_clean.ipynb
│   └── fast_fashion_filter.ipynb
├── dashboard/
│   └── Bahrain_Fast_Fashion.pbix
└── README.md
