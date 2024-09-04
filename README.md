# Bike Sales Dashboard

## Overview
This dashboard provides an interactive visualization of bike sales data, including various metrics and filters to analyze sales performance. It is designed to help users understand key trends and insights related to bike purchases.

## Features
- **Average Income per Purchase**: Bar chart displaying average income per purchase categorized by marital status.
- **Age Bracket Purchased Bike**: Pie chart showing the percentage of bike purchases by different age brackets.
- **Customer Commute**: Line graph comparing the number of bikes sold over time across different education levels.
- **Filters**: Interactive slicers for filtering data by marital status, region, education, and occupation.

## Data Sources
The data used in this dashboard is sourced from the Bike_Buyers sheet within the same Excel file.

## DAX Scripts
The following DAX scripts were used to create new columns and measures:

1. **Age Bracket Categorization**:
   ```DAX
   = IF(L2 > 54, "Old",  IF(L2 >= 31, "Middle Age",  IF(L2 < 31, "Adolescent", "Invalid" )))
   ```
   - This script categorizes ages into three brackets: "Old" for ages above 54, "Middle Age" for ages between 31 and 54, and "Adolescent" for ages below 31. If the age does not fall into any of these categories, it returns "Invalid".

## How to Use
1. **Filters**: Use the slicers on the left side to filter the data by marital status, region, education, and occupation.
2. **Charts**: Interact with the charts to view detailed insights. Hover over the charts to see tooltips with additional information.
3. **Data Table**: View the data table below each chart for detailed data points.

## Publishing
**Tableau Public Link**: [Bike Sales Dashboard on Tableau Public](https://public.tableau.com/app/profile/akram.emrahnejad/vizzes)

