# Monthly Sales Dashboard  
## Regional Revenue & Performance Insights

## Overview
This project analyzes monthly sales performance across regions, stores, and products, and presents the results in an interactive dashboard called **“Regional Revenue Dashboard.”** Users can select a region to explore revenue trends, growth rates, and top/bottom product performance.

## Financial Recommendations

- Prioritise marketing and inventory investment in **New York** and **Los Angeles**, where strong YoY growth indicates greater future revenue potential.
- Conduct a product portfolio review in **Chicago** to identify products that should be repositioned, promoted, discounted, or phased out.
- Implement **region-specific inventory planning** to better align product offerings with local customer preferences.
- Establish an **early-warning monitoring framework** to flag products with consecutive monthly declines before they significantly impact revenue.
- Benchmark top-performing stores and replicate successful operational, merchandising, and promotional practices across lower-performing locations.
- Reduce reliance on mature markets by accelerating growth initiatives in faster-growing regions and diversifying future revenue sources.

## Dataset
The dataset contains **10 key fields**:
- Year
- Month
- Store Name
- Region
- Store Type
- Product Name
- Product Category
- Units Sold
- Revenue
- Profit

It spans **4,795 columns (including headers)**.

<img width="1482" height="572" alt="Screenshot 2026-01-19 175800" src="https://github.com/user-attachments/assets/a09597c8-3bee-4105-a28e-2445be564d23" />

## Data Preparation & Calculations
Key steps included:
- Cleaning and structuring the dataset for analysis
- Filtering and validating **3 unique regions**
- Creating dynamic **date filters**, including:
  - Current Year / Current Month
  - Previous Year / Previous Month
  - Current Period
- Summarising core KPIs:
  - Total Revenue
  - Previous Year Revenue
  - Previous Month Revenue
  - YoY % Change
  - MoM % Change
  - Revenue Trend
- Building store performance views using **10 unique stores**
- Identifying **Top 6** and **Bottom 6** performing products
- Applying Excel formulas to extract and compute metrics:
  - **MAX, MAXIFS, IF, VLOOKUP, SUMIFS, RANK.AVG, INDEX/MATCH**

<img width="762" height="238" alt="image" src="https://github.com/user-attachments/assets/b92e21e8-d90e-4d6c-9c3c-8540ba6aa6fc" />

<img width="416" height="296" alt="image" src="https://github.com/user-attachments/assets/79776741-03fe-480b-95bb-b467b3997aa4" />

## Dashboard Features
The interactive dashboard allows users to choose a region and instantly view:
- **Total revenue** with **MoM** and **YoY % change**
- **Revenue trend** over time
- **Store performance comparisons** across regions
- **Top and bottom products**, including:
  - Revenue
  - MoM revenue change

<img width="2183" height="1051" alt="Screenshot 2026-05-31 223213" src="https://github.com/user-attachments/assets/27883a5f-1bd0-4ff9-ae86-9ae9e9caa023" />
<img width="2190" height="1046" alt="Screenshot 2026-05-31 223224" src="https://github.com/user-attachments/assets/45b00c07-05d4-4dac-98ba-a97dafc8ac3e" />
<img width="2275" height="1071" alt="Screenshot 2026-05-31 224552" src="https://github.com/user-attachments/assets/d990577a-b059-4981-a58e-8b3be6cb10f1" />

## Key Insights

- Chicago generated the highest revenue at **$61.7K**, but it was the only region with both negative month-over-month (**-11.6%**) and year-over-year (**-8.7%**) growth. This suggests that its strong market position is being sustained by historical scale rather than current momentum.
- New York and Los Angeles outperformed Chicago in both MoM and YoY growth, indicating a potential shift in customer demand and future revenue opportunities toward these regions.
- A small number of products contributed disproportionately to both revenue growth and decline, making regional performance highly sensitive to changes in product demand.
- While several Chicago stores maintained strong revenue performance, underperforming products generated significantly greater losses than the gains created by top-performing products, driving the region's overall decline.
- The highest-growth products varied considerably across New York, Los Angeles, and Chicago, suggesting that a single product strategy may not maximize performance across all markets.
- Significant differences in revenue and growth between stores within the same region suggest opportunities to replicate successful practices from top-performing locations.

## Tools & Skills
- **Excel** (MAX, MAXIFS, IF, VLOOKUP, SUMIFS, RANK.AVG, INDEX/MATCH)
- **Data cleaning & preparation**
- **KPI reporting** (MoM, YoY, revenue comparisons)
- **Trend analysis** (revenue trends over time)
- **Interactive dashboard design** (region slicers/filters)
