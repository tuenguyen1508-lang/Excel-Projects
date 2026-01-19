# Monthly Sales Dashboard  
## Regional Revenue & Performance Insights

## Overview
This project analyzes monthly sales performance across regions, stores, and products, and presents the results in an interactive dashboard called **“Regional Revenue Dashboard.”** Users can select a region to explore revenue trends, growth rates, and top/bottom product performance.

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

<img width="598" height="293" alt="image" src="https://github.com/user-attachments/assets/2163a8da-2c84-4846-86a4-f43d7745079e" />

## Key Insight
- **Chicago** had the **highest total revenue**, but revenue **decreased 11.6% MoM** and **8.7% YoY**.  
- **New York** and **Los Angeles** generated lower revenue than Chicago, but both showed **positive MoM and YoY growth**.

## Tools & Skills
- **Excel** (MAX, MAXIFS, IF, VLOOKUP, SUMIFS, RANK.AVG, INDEX/MATCH)
- **Data cleaning & preparation**
- **KPI reporting** (MoM, YoY, revenue comparisons)
- **Trend analysis** (revenue trends over time)
- **Interactive dashboard design** (region slicers/filters)
- **Store & product performance analysis** (top/bottom products, store benchmarking)

