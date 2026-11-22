# India CPI Inflation Analysis

An Excel-based analysis of India's Consumer Price Index (CPI) data, built as a data analyst case study for the National Statistical Office scenario. The project uses formulas, pivot tables, and charts to uncover what drives inflation in India, from category contributions and year-on-year trends to the effect of COVID-19 and global crude oil prices.

---

## Business Context

India measures inflation through the Consumer Price Index (CPI), which tracks the price of a fixed basket of goods and services (food, housing, fuel and light, clothing, transport, health, education, recreation and more). As an analyst at the National Statistical Office, the goal is to find key trends in the CPI data and answer questions a senior stakeholder would ask about inflation.

## Dataset

- **Source:** CPI inflation index data extracted from the Government of India (GOI) website
- **File:** `All_India_Index_Data.xlsx`
- **Contents:** Monthly index values by category for Rural (CPI-R), Urban (CPI-U) and the Combined General Index
- **Data notes:**
  - Each value is an index number, not a price, so index values are never summed across months
  - Missing values were handled with a suitable imputation technique (such as moving averages)
  - For this analysis, all categories are treated with equal weights

## Repository Contents

| File | Description |
|------|-------------|
| `All_India_Index_Data.xlsx` | Raw CPI dataset |
| `India_CPI_Inflation_Final.xlsx` | Final workbook with all working sheets, formulas, pivot tables and charts |

## Problem Statement

### 1. Category contribution to the CPI basket
- Grouped similar categories into broader buckets (for example, Meals, Beverages and Cereals into **Food**)
- Calculated each bucket's contribution for the latest month so that all contributions add up to 100%
- Identified the broader category with the highest contribution

### 2. Year-on-year inflation trend (2017 onwards)
- Calculated Y-o-Y inflation for the combined (rural + urban) General Index
- Plotted the growth rate and identified the year with the highest inflation
- Researched the reasons behind that peak

### 3. Food inflation for the 12 months ending May 2023
- Tracked the month-on-month trend of the broader Food bucket
- Highlighted the months with the highest and lowest food inflation
- Measured absolute changes in inflation and identified the biggest individual contributor within Food

### 4. Impact of COVID-19
- Treated March 2020 (first lockdown) as the onset of the pandemic
- Compared inflation before and after March 2020
- Focused on healthcare, food and essential services

### 5. Imported crude oil prices and inflation
- Analysed month-on-month oil price movements from 2021 to 2023
- Used `CORREL` to measure the relationship between oil price changes and category inflation
- Identified the category most strongly linked to oil price fluctuations

## Key Findings

- **Highest-contributing category:** _[category name, X%]_
- **Year with highest inflation:** _[year, X%]_, driven by _[reason from your research]_
- **Highest food inflation month:** _[month, X%]_
- **Lowest food inflation month:** _[month, X%]_
- **Biggest individual food contributor:** _[item]_
- **COVID-19 effect:** _[inflation before vs after Mar 2020]_
- **Category most correlated with oil prices:** _[category, correlation value]_

## Methodology

- **Month-on-month inflation** = (CPI current month − CPI previous month) / CPI previous month × 100
- **Annual inflation** = (CPI at end of period − CPI at start of period) / CPI at start of period × 100
- **Contribution** = category index share of the total, normalised to 100%
- **Correlation** = Excel's `CORREL` function between oil price change and category inflation

## Tools and Skills Used

- **Microsoft Excel:** formulas, pivot tables, charts
- **Lookup functions:** `VLOOKUP`, `HLOOKUP`, `INDEX-MATCH`
- **Statistics:** `CORREL`, percentage change, moving-average imputation
- **Data cleaning and handling missing values**
- **Data visualisation and storytelling with data**

Connect on [LinkedIn](https://www.linkedin.com/in/prodipta-swarnakar/) 
           [Gmail](prodiptaswarnakar@gmail.com)   
---
