# Customer Insights Dashboard (Power BI + Python)

## Overview
Analyzed **2,500+ retail transactions** to surface trends across **time**, **product categories**, **demographics**, and **day-of-week**.  
Built an end-to-end workflow with **Python (Pandas, Matplotlib)** for cleaning/EDA and **Power BI** for interactive reporting.

**KPI Snapshot (from dashboard)**
- **Total Revenue:** ~$456K  
- **Transaction Count:** ~1K  
- **Average Order Value:** ~$456

**Quick Links**
- Notebook → [notebooks/retail_analysis.ipynb](notebooks/retail_analysis.ipynb)  
- Dashboard (PDF) → [visuals/retail_bi.pdf](visuals/retail_bi.pdf)

> PBIX can be large; the PDF provides an instant preview.

---

## Executive Insights
- **Seasonality:** Peak in **May (~$53K)** → spring promo window & inventory ramp.
- **Category Mix:** **Electronics** and **Clothing** lead (each **>$156K**).
- **Core Segment:** **Ages 36–50** contribute the most revenue.
- **Gender Split:** ~**51% Female / 49% Male** → balanced creative and targeting.
- **Timing:** Thu–Sun stronger → schedule ads, staffing, and flash promos accordingly.

---

## Notebook Highlights
- Cleaned transactions (types, duplicates, nulls) and standardized column names.
- Engineered features (year/month/day, **day_of_week**, **age groups**).
- Built core cuts: monthly trend, category mix, gender split, age cohorts, day-of-week.
- Exported clean CSVs for Power BI refresh: `monthly_sales.csv`, `category_revenue.csv`, `age_gender_revenue.csv`, `dow_revenue.csv`.

<details>
  <summary>Details (optional)</summary>

**Cleaning:** parsed dates; de-duped; validated numeric fields (`quantity`, `price_per_unit`, `total_amount`).  
**Features:** derived time buckets & age bins (18–25, 26–35, 36–50, 51+).  
**Aggregations:** month trend, category mix, gender split, age cohorts, DOW (Mon→Sun).  
**Outputs:** CSVs decouple EDA from BI for repeatable, lightweight dashboard refreshes.

</details>

---

## Power BI Report
KPI tiles, monthly trend, category mix, demographic breakdowns, and day-of-week comparison.  
Open **`visuals/retail_bi.pdf`** for a quick snapshot.

---
