<div align="center">
# Blinkit Sales Analysis Dashboard
 
### An interactive Excel dashboard for retail sales, outlet performance, and product insights

<div align="center">

# Blinkit Sales Analysis Dashboard

### An interactive Excel dashboard for retail sales, outlet performance, and product insights


</div>

---

## Table of Contents

- [Overview](#overview)
- [Dashboard Preview](#dashboard-preview)
- [Business Objectives](#business-objectives)
- [Key Performance Indicators](#key-performance-indicators)
- [Dashboard Features](#dashboard-features)
- [Key Insights](#key-insights)
- [Dataset](#dataset)
- [Data Preparation](#data-preparation)
- [Tools and Techniques](#tools-and-techniques)
- [Repository Structure](#repository-structure)
- [How to Use](#how-to-use)
- [Recommendations](#recommendations)
- [Future Enhancements](#future-enhancements)
- [Author](#author)

---

## Overview

This project is an interactive sales analysis dashboard built entirely in **Microsoft Excel** using Blinkit grocery data. It analyzes **8,523 items** across outlets of different sizes, locations, and formats, turning raw transactional data into a clear, decision-ready view.

The dashboard combines KPI cards, pivot-chart visuals, and a slicer-based filter panel, so stakeholders can explore performance by outlet size, location tier, and item type without writing a single formula.

---

## Dashboard Preview

<img width="800" height="423" alt="Dashboard_Preview" src="https://github.com/user-attachments/assets/85409faa-8e41-41aa-8071-ffbeba43afe4" />

> The filter panel on the left updates every chart and KPI card at once. The preview above shows the dashboard filtered by outlet size.

---

## Business Objectives

1. Track overall sales performance through headline KPIs.
2. Identify the best performing product categories and outlet formats.
3. Understand how outlet size, location tier, and establishment year affect sales.
4. Compare sales of Low Fat and Regular products across locations.
5. Provide an interactive tool for fast, self-service analysis.

---

## Key Performance Indicators

| KPI | Value (All Data) | Description |
|-----|------------------|-------------|
| **Total Sales** | $1.20M | Total revenue across all items |
| **Average Sales** | $141 | Mean sales value per item |
| **Number of Items** | 8,523 | Total items analyzed |
| **Average Rating** | 4.0 | Mean customer rating |

> KPI cards update dynamically when filters are applied. For example, filtering for Small outlets shows $0.25M total sales across 1,753 items with a 3.9 average rating.

---

## Dashboard Features

| Section | What It Shows |
|---------|---------------|
| **KPI Cards** | Total Sales, Average Sales, Number of Items, Average Rating |
| **Filter Panel** | Slicers for Outlet Size, Outlet Location, and Item Type |
| **Fat Content** | Low Fat vs Regular share of sales (donut chart) |
| **Fat by Outlet** | Fat content sales across Tier 1, 2, and 3 locations |
| **Item Type** | Sales ranked across 15 product categories |
| **Outlet Size** | Sales split across High, Medium, and Small outlets |
| **Outlet Location** | Sales comparison by location tier |
| **Outlet Type** | Total sales, average sales, and item count by outlet format |
| **Outlet Establishment** | Sales trend by outlet establishment year (2011 to 2022) |

**Design highlights:** consistent Blinkit-inspired yellow and green theme, rounded KPI cards with icons, clean chart styling, and one-click navigation icons.

---

## Key Insights

- **Regular fat items drive 65% of sales** ($776.3K) compared with 35% for Low Fat ($425.4K).
- **Fruits & Vegetables ($178.1K) and Snack Foods ($175.4K)** are the top two item types, followed by Household ($136.0K).
- **Medium outlets lead with 42% of sales** ($507.9K), followed by Small (37%) and High (21%).
- **Tier 3 locations generate the most sales** ($472.1K), ahead of Tier 2 ($393.2K) and Tier 1 ($336.4K).
- **Supermarket Type 1 dominates outlet formats** with $787.5K and 5,577 items.
- **Average sales per item is stable** at about $140 across all outlet types, so volume rather than price drives the differences.
- **Outlets established in 2018 show the sales peak** ($204.5K).

---

## Dataset

| Attribute | Details |
|-----------|---------|
| **Source** | Blinkit Grocery Dataset ([Kaggle / other source]) |
| **Records** | 8,523 items |
| **Key Fields** | Item Type, Item Fat Content, Outlet Size, Outlet Location Type, Outlet Type, Outlet Establishment Year, Sales, Rating |

The workbook contains three sheets: **BlinkIT Grocery Data** (raw data), **Sheets Design** (pivot tables and chart calculations), and **Dashboard** (final interactive view).

---

## Data Preparation

- Standardized Fat Content labels (for example, "LF" and "low fat" to **Low Fat**, "reg" to **Regular**)
- Checked for duplicates, blanks, and inconsistent formatting
- Handled missing values in fields such as Item Weight
- Structured the data as an Excel Table for dynamic pivot refresh
- Validated pivot totals against the raw data

---

## Tools and Techniques

- **Microsoft Excel** for analysis and dashboard design
- **Pivot Tables and Pivot Charts** for aggregation and visualization
- **Slicers** connected across multiple pivots for unified filtering
- **KPI cards** built from pivot and formula outputs
- **Data cleaning and transformation** using Excel functions and tools
- **Custom formatting and layout** for a polished, branded interface

---

## Repository Structure

```
Blinkit-Sales-Analysis-Excel-Dashboard/
│
├── Data/
│   └── Blinkit_Grocery_Data.xlsx
│
├── Dashboard/
│   └── Blinkit_Sales_Dashboard.xlsx
│
├── Images/
│   └── Dashboard_Preview.gif
│
└── README.md
```

---

## How to Use

1. **Download** `Blinkit Grocery Data Excel.xlsx` from this repository.
2. Open it in **Microsoft Excel** (2016 or later recommended).
3. Go to the **Dashboard** sheet.
4. Use the **Filter Panel** on the left to select outlet size, location, or item type.
5. Watch the KPI cards and charts update instantly. Use the clear-filter icon on each slicer to reset.

> Slicers require desktop Excel. Some features may not display correctly in Excel Online or mobile viewers.

---

## Recommendations

- **Prioritize inventory** for Fruits & Vegetables and Snack Foods, the two top-selling categories.
- **Focus expansion on Tier 3 locations**, which lead in sales.
- **Replicate the Supermarket Type 1 model**, which generates the bulk of revenue.
- **Strengthen Low Fat offerings**, which hold only 35% of sales and may have room to grow.
- **Investigate high-performing establishment years** such as 2018 to understand what drove the peak.

---

## Future Enhancements

- Build an equivalent dashboard in Power BI and Tableau for comparison
- Add profit and margin analysis
- Include sales forecasting and trend projections
- Add item-level drill-through for deeper analysis

---

<div align="center">

If you found this project useful, please consider giving it a star.

</div>
