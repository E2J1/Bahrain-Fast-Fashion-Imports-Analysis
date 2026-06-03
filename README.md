# Bahrain Fast Fashion Market Intelligence Report (2021–2025)

A market intelligence and business intelligence project analyzing Bahrain's fast fashion import trends to support a data-driven market entry strategy for a new apparel retailer.

---

## Project Overview

This project was developed as part of a simulated consulting engagement for a fictional GCC market intelligence firm, **Gulf Vision Consulting**.

The client, **ROVE**, is a proposed fast fashion retailer planning to enter Bahrain's apparel market.

The analysis focused on five years of official Bahrain import data (2021–2025) to uncover demand trends, supplier sourcing opportunities, seasonal inventory patterns, import costs, and trade logistics.

The final deliverable combined Python-based data preparation with an interactive Power BI executive dashboard.

---

## Business Problem & Client

### Business Problem

ROVE lacked visibility into:

- Which apparel categories dominate Bahrain's import market
- Which sourcing countries provide the best cost efficiency
- Which months experience peak seasonal demand
- Which product categories present the strongest commercial opportunity
- How import trends evolved between 2021–2025

Without data-driven visibility, inventory planning, sourcing strategy, and pricing decisions carried significant commercial risk.

This project transformed raw Bahrain import data into strategic business intelligence to support a confident market entry strategy.

### Client Profile

**Client Type:** A new fast fashion retailer planning to enter the Bahraini apparel market.

**Business Goals:**
- Identify high-demand apparel categories
- Source inventory from cost-efficient supplier countries
- Understand seasonal demand behavior
- Build a competitive pricing strategy
- Reduce inventory and sourcing risks

**Target Market:**
- Young adults and trend-focused consumers
- Mid-range affordable fashion segment
- Seasonal and fast-moving apparel products

---

## Business Questions

- Which apparel categories generate the highest import value?
- Which products dominate import volume?
- Which supplier countries provide the lowest average cost per item?
- How has Bahrain's apparel market grown between 2021–2025?
- Which months and seasons experience peak demand?
- Which categories present premium market opportunities?
- Which sourcing markets provide the best balance between cost and lead time?

---

## Data Source

The dataset was obtained from the Bahrain Open Data Portal and contains official Bahrain import records between 2021 and 2025.

**Source:** https://www.data.gov.bh/explore/?disjunctive.theme&sort=modified&q=imports

**Dataset Coverage:**
- Import transactions
- Commodity classifications (HS Codes)
- Supplier countries
- Import values
- Import quantities and weights
- Monthly import activity

### Data Dictionary

| Column Name | Type | Description |
|-------------|------|-------------|
| `year` | int | Year of the import record. |
| `month` | str | Month when the import transaction was recorded. |
| `commodity_no` | str / int | Commodity classification code used to identify the apparel product type. |
| `commodity` | str | Description of the imported clothing item. |
| `un_code` | str | Country code of the exporting/supplier country. |
| `country_name` | str | Name of the country exporting the apparel products to Bahrain. |
| `import_value_bd` | float | Import value measured in Bahraini Dinar (BD). |
| `import_value_usa` | float | Import value converted to US Dollars (USD). |
| `import_weight_kg` | float | Total imported weight measured in kilograms. |
| `import_quantity` | int / float | Number of imported units/items. |
| `um` | str | Unit of measurement used for the imported quantity, such as number of items (`NO`). |

---

## Tech Stack & Methodology

### Data Preparation (Python)
- Combined 2021–2025 import datasets
- Cleaned commodity descriptions and removed newline characters
- Standardized HS commodity codes and country naming
- Created calculated business metrics
- Built seasonal classifications
- Derived clothing categories from commodity descriptions

**Libraries:** Python, Pandas

### Dashboard Development (Power BI)
- Custom DAX KPI measures
- Conditional formatting logic
- Seasonal trend calculations
- Dynamic filtering and sourcing analysis
- Business-focused data modeling
- Commodity heatmaps and supplier benchmarking

---

## Executive Dashboard Preview

![Executive Dashboard](images/dashboard-overview.png)

![Dashboard Demo](images/dashboard-demo.gif)

> Interactive Power BI dashboard featuring seasonal filters, sourcing analysis, KPI tracking, heatmaps, and clothing category insights.

---

## Key Insights

### Market Growth

![Market Growth](images/market-growth.png)

- Bahrain's apparel import value increased by approximately **41%** between 2021 and 2025
- Total import value peaked at **BD 87M** in 2024
- Growth remained consistent across multiple years, signaling sustained market demand
- Total import quantity exceeded **107M units** across the analysis period

### Commodity Analysis

![Commodity Analysis](images/commodity-analysis.png)

**Highest Import Value Categories:**
- Trousers & Shorts — BD 96M
- Dresses — BD 74M
- T-shirts — BD 65M

**Key Findings:**
- T-shirts dominated import volume but operated on thinner margins
- Dresses showed strong premium positioning potential
- Trousers & Shorts represented the largest commercial opportunity

### Supplier Country Analysis

![Country Analysis](images/country-analysis.png)

- China dominated total import value
- India and Bangladesh offered the lowest average cost per item (~BD 2)
- Italy operated as a premium-priced supplier market
- India and Bangladesh provide the strongest balance between low sourcing cost, shorter lead times, and high manufacturing volume

### Seasonal Demand

- Demand peaks occurred during January–March and December
- Seasonal patterns remained consistent across multiple years
- Retailers should align supplier ordering cycles during October–November to ensure inventory arrives before peak demand periods

### Logistics & Import Operations

- Sea freight was the most cost-effective option for bulk inventory imports
- Air freight was best suited for urgent trend-reactive replenishment
- Bahrain's apparel imports are subject to customs duties and VAT charges

---

## Strategic Recommendations

![Strategic Recommendations](images/recommendations.png)

**Product Strategy:** Focus on T-shirts, Trousers & Shorts, and Dresses — the categories that consistently dominated Bahrain's import market.

**Sourcing Strategy:**
- Source core inventory from India and Bangladesh for lowest cost per unit
- Use China for high-variety trend-driven inventory
- Delay premium sourcing markets until brand positioning matures

**Inventory Timing:** Align purchasing cycles around Q1 and December demand peaks to optimize stock availability and reduce shortages during high-demand periods.

---

## Limitations

- The dataset only includes import activity and does not include local retail sales performance
- Import data reflects wholesale and landed costs rather than consumer pricing
- Some commodity descriptions were generalized, limiting product-level precision
- Visual apparel style classifications were unavailable
- Gender demand segmentation could not be validated using consumer sales data
- Inflation, logistics disruptions, and macroeconomic variables were not included

---

## Future Improvements

- Integrate retail sales and customer behavior data
- Include forecasting models for seasonal demand
- Add supplier risk analysis and logistics KPIs
- Incorporate product image classification models
- Develop automated Power BI refresh pipelines

---

## Repository Structure

```bash
.
├── data/
├── images/
│   ├── dashboard-overview.png
│   ├── dashboard-demo.gif
│   ├── market-growth.png
│   ├── commodity-analysis.png
│   ├── country-analysis.png
│   ├── recommendations.png
│   └── dax-measures.png
├── notebooks/
│   ├── bahrain_imports_clean.ipynb
│   └── fast_fashion_filter.ipynb
├── dashboard/
│   └── Bahrain_Fast_Fashion.pbix
└── README.md
```


---

## Author

**Ebrahim Alsawan**

Data Analyst | Business Intelligence Analyst

LinkedIn: https://www.linkedin.com/in/ebrahim-alsawan-a6977a2b9/

GitHub: https://github.com/E2J1
