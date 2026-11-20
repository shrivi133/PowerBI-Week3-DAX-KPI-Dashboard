# Power BI Week 3 — DAX Functions & KPI Visuals (Retail Store Dashboard)

## Project Overview
This repository contains the **Week 3: DAX Functions & KPI Visuals** Power BI assignment[cite: 11]. It implements core DAX aggregations, ratio calculations, interactive slicers, conditional formatting rules, and an executive **Retail Store KPI Dashboard**[cite: 11].

---

## Implemented Assignment Requirements[cite: 11]

### 1. DAX Measures
| Measure Name | DAX Formula | Computed Value |
| :--- | :--- | :--- |
| **Total Sales**[cite: 11] | `Total Sales = SUM(Sales[Sales])`[cite: 11] | `$17,240.00` |
| **Total Profit**[cite: 11] | `Total Profit = SUM(Sales[Profit])`[cite: 11] | `$3,035.00` |
| **Profit Margin**[cite: 11] | `Profit Margin = DIVIDE([Total Profit], [Total Sales])`[cite: 11] | `17.60%` |

### 2. Dashboard Visuals & Interactive Controls[cite: 11]
* **3 KPI Cards:** Displays `Total Sales` (`$17,240.00`), `Total Profit` (`$3,035.00`), and `Profit Margin` (`17.60%`)[cite: 11].
* **Interactive Slicers & Filters:** Configured slicers for **Region** (`North`, `South`, `East`, `West`), **Year** (`2024`, `2025`), and **Category** (`Technology`, `Furniture`, `Office Supplies`)[cite: 11].
* **Conditional Formatting:** Applied rules on Profit visuals and tables to highlight **negative profits (`< 0`) in red** (flagging discounted `Furniture` orders with negative margins)[cite: 11].
* **Bar & Line Charts:** Category/Regional performance bar charts and monthly sales trend line charts[cite: 11].

---

## Analytical Summary

### Performance by Region
| Region | Total Sales ($) | Total Profit ($) |
| :--- | :--- | :--- |
| **South** | `$5,140.00` | `$865.00` |
| **West** | `$4,440.00` | `$630.00` |
| **North** | `$4,130.00` | `$660.00` |
| **East** | `$3,530.00` | `$880.00` |

### Performance by Category (Conditional Formatting Highlight)
| Category | Total Sales ($) | Total Profit ($) | Status |
| :--- | :--- | :--- | :--- |
| **Technology** | `$11,800.00` | `$2,810.00` | Positive Profit |
| **Office Supplies** | `$2,030.00` | `$560.00` | Positive Profit |
| **Furniture** | `$3,410.00` | `-$335.00` | **Negative Profit (Highlighted Red)**[cite: 11] |

---

## Repository Files
* `README.md` — Project documentation, KPI summary, and conditional formatting breakdown.
* `DAX_Measures_Week3.dax` — All DAX measures (`SUM`, `DIVIDE`, `SUMX`, `AVERAGE`, `CALCULATE`) and conditional formatting color rules[cite: 11].
* `Retail_Sales_Data.csv` — Retail sales dataset with `Order Date`, `Region`, `Category`, `Sales`, `Profit`, `Quantity`, and `Discount` columns[cite: 11].