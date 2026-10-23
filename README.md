# Blinkit Sales Analysis Dashboard (Excel)

An interactive Excel dashboard that analyzes Blinkit retail sales data across
8,523 items, covering total sales of $1.20M, an average sale of $141, and an
average customer rating of 4.0.

# Excel Dashboard

<img width="800" height="423" alt="Dashboard_Preview" src="https://github.com/user-attachments/assets/85409faa-8e41-41aa-8071-ffbeba43afe4" />


## Objective
Identify which products, outlet types, and locations drive sales, so that
inventory and outlet strategy decisions can be data-backed.

## Dashboard Features
- **KPI cards:** Total Sales, Average Sales, Number of Items, Average Rating
- **Filter panel:** Slicers for Outlet Size, Outlet Location, and Item Type
- **Fat Content:** Low Fat vs Regular sales split (35% vs 65%)
- **Fat by Outlet:** Fat content sales across Tier 1, 2, and 3 locations
- **Item Type:** Sales ranked across 15 product categories
- **Outlet Size:** Sales split across High, Medium, and Small outlets
- **Outlet Location:** Sales comparison across Tier 1, 2, and 3 cities
- **Outlet Type:** Total sales, average sales, and item count by outlet format
- **Outlet Establishment:** Sales trend by year of outlet establishment (2011-2022)

## Key Insights
- Regular fat items generate about 65% of total sales ($776.3K).
- Fruits & Vegetables ($178.1K) and Snack Foods ($175.4K) are the top item types.
- Medium-sized outlets contribute the most sales (42%, $507.9K).
- Tier 3 locations lead in sales ($472.1K), ahead of Tier 2 and Tier 1.
- Supermarket Type 1 dominates outlet type sales ($787.5K).
- Outlets established in 2018 show the sales peak ($204.5K).

## Tools & Techniques
- Microsoft Excel
- Data cleaning and transformation
- Pivot tables and pivot charts
- Slicers for interactive filtering
- Custom dashboard design with KPI cards

## Files
- `Blinkit Glocery Data Excel.xlsx`: raw dataset
- `Blinkit Glocery Data Excel.xlsx`: final dashboard
- `Dashboard_Preview.gif`: dashboard screenshot

## How to Use
1. Download `Blinkit Glocery Data Excel.xlsx`.
2. Open it in Excel (2016 or later recommended).
3. Use the filter panel on the left to explore by outlet size, location, or item type.

## Business Questions
- Which item categories generate the highest sales?
- How do outlet size and location tier affect revenue?
- Does fat content influence sales across different locations?
- How has performance varied by outlet establishment year?

## Dataset
- **Source:** Kaggle - Blinkit Grocery Dataset
- **Records:** 8,523 items
- **Key Fields:** Item Type, Fat Content, Outlet Size, Outlet Location Type,
  Outlet Type, Establishment Year, Sales, Rating

## Data Cleaning
- Standardized Fat Content values ("LF", "low fat" → "Low Fat"; "reg" → "Regular")
- Handled missing values in Item Weight and Outlet Size
- Checked for duplicates and inconsistent formatting

## Recommendations
- Prioritize Fruits & Vegetables and Snack Foods inventory in high-performing outlets.
- Focus expansion on Tier 3 locations, which lead in total sales.
- Study what makes Supermarket Type 1 outlets succeed and replicate it in other formats.

## Future Improvements
- Build the same dashboard in Power BI for comparison
- Add a profit and margin analysis
- Include sales forecasting

