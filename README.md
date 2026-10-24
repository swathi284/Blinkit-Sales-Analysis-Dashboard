<div align="center">

# BlinkIT Grocery Sales Analysis Dashboard

**An interactive Excel dashboard that analyses grocery sales, customer ratings, and outlet performance across 8,500+ product records.**

![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![Pivot Tables](https://img.shields.io/badge/Pivot%20Tables-1F4E78?style=for-the-badge)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-F8C400?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

</div>

---

## Table of Contents

- [Overview](#overview)
- [Business Problem](#business-problem)
- [Dashboard Preview](#dashboard-preview)
- [Key Performance Indicators](#key-performance-indicators)
- [Dataset](#dataset)
- [Data Preparation](#data-preparation)
- [Analysis Performed](#analysis-performed)
- [Key Insights](#key-insights)
- [Recommendations](#recommendations)
- [Tools & Techniques](#tools--techniques)
- [Project Structure](#project-structure)
- [How to Use](#how-to-use)
- [Future Enhancements](#future-enhancements)
- [License](#license)

---

## Overview

This project analyses grocery sales data from **BlinkIT**, an Indian quick-commerce grocery delivery platform. Using **Microsoft Excel**, the raw data is cleaned, summarised with **PivotTables**, and presented in an interactive **dashboard with slicers**, so business users can filter and explore performance by item, outlet, and location without writing any formulas.

---

## Business Problem

BlinkIT's management needs a clear view of how the business is performing across product categories and outlet types. This dashboard helps answer:

- What are the **total sales, average sales, and customer rating** overall?
- Which **item types** generate the most revenue?
- How do **low-fat and regular** products compare in sales?
- Which **outlet size, location tier, and outlet type** perform best?
- How does **outlet age (establishment year)** relate to sales?

---

## Dashboard Preview

<img width="800" height="423" alt="Blinkit_Analysis_Preview" src="https://github.com/user-attachments/assets/cc6ef985-a4d8-4223-8cdd-02731a45b009" />

---

## Key Performance Indicators

| KPI | Value |
|---|---|
| **Total Sales** | 1.20M (1,201,681) |
| **Average Sales per Item** | 140.99 |
| **Number of Items** | 8,523 |
| **Average Customer Rating** | 3.97 / 5 |

---

## Dataset

**File:** `BlinkIT_Grocery_Data_Excel.xlsx` | **Records:** 8,523 | **Columns:** 12

| Column | Description |
|---|---|
| `Item Identifier` | Unique product ID |
| `Item Type` | Product category (16 categories, e.g., Dairy, Snack Foods) |
| `Item Fat Content` | Low Fat or Regular |
| `Item Weight` | Weight of the product |
| `Item Visibility` | Share of display area allocated to the product |
| `Outlet Identifier` | Unique outlet ID |
| `Outlet Establishment Year` | Year the outlet was established |
| `Outlet Size` | Small, Medium, or High |
| `Outlet Location Type` | Tier 1, Tier 2, or Tier 3 |
| `Outlet Type` | Grocery Store or Supermarket Type 1/2/3 |
| `Sales` | Sales value of the item |
| `Rating` | Customer rating |

---

## Data Preparation

| Step | Detail |
|---|---|
| **Standardised categories** | `Item Fat Content` contained inconsistent labels (`Low Fat`, `low fat`, `Regular`). These were consolidated into two clean categories: **Low Fat** and **Regular**. |
| **Missing values** | `Item Weight` has 1,463 blank values (~17%). These were left untouched because weight is not used in any dashboard measure. |
| **Validation** | Checked all other columns for nulls and inconsistencies. No further issues were found. |
| **Modelling** | Cleaned data was converted to a structured table and used as the single source for all PivotTables. |

---

## Analysis Performed

The workbook is organised into three sheets:

| Sheet | Purpose |
|---|---|
| **BlinkIT Grocery Data** | Cleaned source data |
| **Sheets Design** | PivotTables and supporting calculations for every chart and KPI |
| **Dashboard** | Final interactive dashboard with KPI cards, charts, and slicers |

**Analyses included:**

- Total Sales by **Fat Content**
- Fat Content by **Outlet Location** (Tier 1 / 2 / 3)
- Total Sales by **Item Type**
- Total Sales by **Outlet Establishment Year**
- Sales by **Outlet Size**
- Sales by **Outlet Location**
- All metrics by **Outlet Type** (Total Sales, Average Sales, Number of Items)

---

## Key Insights

### Product Performance
- **Fruits and Vegetables (178.1K)** and **Snack Foods (175.4K)** are the top two categories, together contributing about **29%** of total sales.
- **Household (136.0K)** and **Frozen Foods (118.6K)** follow.
- **Seafood (9.1K)**, **Breakfast (15.6K)**, and **Starchy Foods (21.9K)** are the lowest-performing categories.

### Fat Content
- **Low Fat items generate 776.3K (about 65%)** of sales, compared with 425.4K for Regular items.
- This pattern holds across all three location tiers, with Low Fat leading in each.

### Outlet Performance
- **Medium-sized outlets** lead with **507.9K (about 42%)**, followed by Small (444.8K) and High (249.0K).
- **Tier 3 locations** generate the most sales (472.1K), followed by Tier 2 (393.2K) and Tier 1 (336.4K).
- **Supermarket Type 1** dominates with **787.5K (about 66%)** of total sales. Grocery Stores (151.9K), Type 2 (131.5K), and Type 3 (130.7K) are far behind.

### Outlet Age
- Outlets established in **2018** have the highest sales at **204.5K**, driven by a higher number of item records (1,463).
- Outlets from **2011** have the lowest sales (78.1K).

### Important Observation
- **Average sales per item (about 140 to 142) and average rating (about 3.95 to 4.0) are nearly identical across all outlet types, sizes, and tiers.** Differences in total sales are therefore driven mainly by **the number of items sold**, not by higher prices or better ratings.

---

## Recommendations

1. **Focus inventory and promotions on top categories**, especially Fruits and Vegetables, Snack Foods, and Household.
2. **Expand the Low Fat range**, as it already accounts for roughly two-thirds of sales.
3. **Prioritise Tier 3 locations and Medium-sized outlets** for growth, since they drive the largest share of sales.
4. **Study the Supermarket Type 1 model** and assess whether its practices can be applied to other outlet types.
5. **Review low-performing categories** such as Seafood and Breakfast to decide whether to promote, bundle, or reduce stock.
6. **Improve customer ratings.** The average of 3.97 is flat across all segments, so a quality or service improvement programme could raise satisfaction everywhere.

---

## Tools & Techniques

| Category | Details |
|---|---|
| Software | Microsoft Excel |
| Analysis | PivotTables, Pivot Charts, Slicers |
| Data Cleaning | Standardising text values, handling missing data, Excel Tables |
| Visualisation | KPI cards, bar charts, column charts, donut/pie charts, interactive filters |

---

## Project Structure

```
blinkit-sales-analysis/
│
├── BlinkIT_Grocery_Data_Excel.xlsx    # Data, pivot tables, and dashboard
├── images/
│   └── dashboard.png                  # Dashboard screenshot
└── README.md
```

---

## How to Use

1. **Clone or download** the repository:
   ```bash
   git clone https://github.com/swathi284/Blinkit-Sales-Analysis-Dashboard.git
   ```
2. Open `BlinkIT Grocery Data Excel.xlsx` in **Microsoft Excel** (2016 or later recommended).
3. Go to the **Dashboard** sheet.
4. Use the **slicers** to filter by item, outlet, and location, and watch the KPIs and charts update.
5. Open the **Sheets Design** sheet to see the PivotTables behind each visual.

---

## Future Enhancements

- Rebuild the dashboard in **Power BI or Tableau** for richer interactivity and sharing.
- Add **time-based analysis** with order dates to study trends and seasonality.
- Add **profit and cost data** to analyse margins, not just sales.
- Build **customer segmentation** and repeat-purchase analysis.
- Automate data refresh with **Power Query**.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">

If you found this project useful, please consider giving it a star.

</div>
