## SUPERSTORE-SALES ANALYSIS

### Project Overview

This project aims to gather insights about the sales performance of a large retail store in recent years. By examining different elements of the sales data, the project aims to identify patterns, offer data-driven suggestions, and develop a more comprehensive understanding of the store's overall performance. 

### Data sources

The primary dataset used for this analysis is the "Superstore" dataset from Excel's sample datasets" file, containing detailed information about each sale made by the company

### Tools used
- Excel - Data Cleaning and Visualization

- Power Bi - Building Visuals

- SQL- Writing queries

### Data Cleaning/Preparation
In the initial data-cleaning phase, we performed the following tasks;
- Data loading and inspection
- Handling inconsistent values
- Data cleaning and formatting\

### Expository Data Analysis(EDA)- Excel
EDA involved exploring the sales data to answer key questions, such as;
- The highest and lowest sales
- The number of orders
- Total sales for the Technology category



### Expository Data Analysis(EDA)- SQL
EDA involved exploring the sales data to answer key questions, such as;
- total count of orders.
-  total profit by Category ordered from highest to lowest profit.


### Data Analysis
```SQL
SELECT COUNT(DISTINCT ORDER_ID)  AS [TOTAL ORDERS]
FROM SUPERSTORES


SELECT CATEGORY, SUM (PROFIT) AS TOTAL_PROFIT
 FROM SUPERSTORES
 GROUP BY CATEGORY
 ORDER BY TOTAL_PROFIT DESC;
```


