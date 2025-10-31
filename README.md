# sales-dashboard-analytics-case-study
Here is a detailed README template for your GitHub repository, based on your attached workflow:

***

# Sales Data Analytics Project

This repository showcases an end-to-end data analytics case study using spreadsheet tools, SQL, and Tableau. The objective is to analyze and visualize sales data using the OSEMN framework to simulate real-world business analytics.

***

### Table of Contents

- Project Overview
- Data Overview
- Workflow & Methodology
  - Scrub (Data Cleaning)
  - Explore (Analysis & SQL)
  - Visualize (Charts & Dashboard)
- Key Results
- How to Reproduce
- References & Credits

***

### Project Overview

This project demonstrates the process of analyzing raw sales data to produce actionable business insights. Starting with a messy dataset, the analysis covers data cleaning, exploration with spreadsheet functions and SQL queries, and visualization using charts and an interactive Tableau dashboard.[1]

***

### Data Overview

- **Source:** Provided raw sales dataset (or sample version)
- **Structure:** Columns with transaction details such as Item Price, Quantity Sold, Sales Date, Product Line, Customer ID, etc.
- **Common Issues:** Missing values, incomplete product information, missing customer IDs, incomplete size records.[1]

***

### Workflow & Methodology

#### Scrub (Data Cleaning)

- Identified and documented common data issues:
  - Missing product names, product lines, and product categories
  - Missing customer IDs and size records
- Cleaning actions taken:
  - Deleted duplicate transaction rows
  - Used filter and group functions to fill in missing cells
  - Deleted rows with missing customer IDs
  - Filled size gaps with “NA” if not relevant for further analysis.[1]

#### Explore (Analysis & SQL)

- Spreadsheet functions applied:
  - `AVERAGE`: Average sales calculated per column
  - `MAX`: Found maximum item price
  - `Product`: Created 'Sales' column by multiplying item price with quantity sold
  - `WEEKDAY` and formatting: Added day-of-week column
  - `CORREL`: Calculated correlation between day of week and sales (correlation constant: -0.078, indicating little/no relationship)[1]
- SQL queries used:
  - Selected top 10 order values: `SELECT D, F, K ORDER BY K DESC LIMIT 10`
  - Item sales counts: `SELECT D, COUNTD GROUP BY D ORDER BY COUNTD DESC`
  - Top selling items: `SELECT D, SUMK GROUP BY D ORDER BY SUMK DESC LIMIT 10`
- Charts:
  - Example: Bar chart showing sales trends by month/weekday.[1]

#### Visualize (Charts & Dashboard)

- Created a Tableau dashboard with:
  - At least two charts displaying sales KPIs and product performance
  - One interactive element for deeper data exploration
- Public dashboard link:  
  `https://public.tableau.com/app/profile/palash.gandhi/viz/SalesDashboard17618350797700/SalesDashboard?publish=yes`[1]
- Included a screenshot/image of the dashboard for reference.[1]

***

### Key Results

- Clean dataset ready for analysis
- Calculated average and max item price, average order value and quantity
- Discovered sales patterns and top-selling products
- Quantified relationships (such as no significant correlation between weekday and sales)
- Delivered professional dashboard highlighting actionable sales KPIs and insights.[1]

***

### How to Reproduce

1. Clone this repository.
2. Review the raw dataset in `/data/raw/`.  
3. Follow data cleaning steps in README and workflow files.
4. Use sample Google Sheets formulas and SQL scripts located in `/analysis/`.
5. Explore provided charts in `/visualizations/`.
6. Open Tableau workbook in `/tableau/` or view published dashboard online.

***

### References & Credits

- Coursera Data Analytics Course project template
- Tableau Public  
- Spreadsheet and SQL functions  
- Project author: Palash Gandhi  
- Data source anonymized for privacy

***

