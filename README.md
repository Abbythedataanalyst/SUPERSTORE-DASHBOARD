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
In the initial data-cleaning phase, I performed the following tasks;
- Data loading and inspection
- Handling inconsistent values
- Data cleaning and formatting

### Expository Data Analysis(EDA)- Excel
EDA involved exploring the sales data to answer key questions, such as;
- The highest and lowest sales
- The number of orders
- Total sales for the Technology category
  
<img width="950" alt="Superstores Dashboard (Excel)" src="https://github.com/Abbythedataanalyst/SUPERSTORE-DASHBOARD/assets/158297673/e3f39eba-ce06-4395-b943-0411f2bb0a54">

### Expository Data Analysis(EDA)- Power Bi
EDA involved exploring the sales data to answer key questions, such as;

- Total sales and profit by Category and Segment
- Sales trended over time  
- Top 5 most profitable products
  
<img width="592" alt="Superstores Dashboard(Power BI)" src="https://github.com/Abbythedataanalyst/SUPERSTORE-DASHBOARD/assets/158297673/f79eb8a6-23f0-4e9f-9a1d-f9f4e562fd1e">

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
### Reviews/Findings

- The analysis revealed fluctuations in sales trends over time, with periods of growth and decline. Understanding these trends can help the store anticipate demand and adjust strategies accordingly.

- By examining sales and profit data by category and segment, the project identified the most profitable areas of the business. This insight can inform resource allocation and marketing efforts to maximize profitability.

- The identification of the top five most profitable products provides valuable information for inventory management and marketing strategies. Focusing on these high-performing products will drive sales and improve overall revenue.

### Recommendations

- Strategic Planning: Based on the findings, it is recommended that the store develop a strategic plan to capitalize on periods of growth and mitigate challenges during downturns. This could include adjusting inventory levels, launching targeted promotions, and optimizing pricing strategies.

- Category Optimization: Leveraging insights from the analysis, the store should consider allocating resources towards categories and segments with the highest profitability. Additionally, efforts should be made to identify and address underperforming categories to improve overall sales performance.

### Limitations

- The analysis focuses primarily on sales data and may not capture other factors that influence store performance, such as marketing campaigns, competitor actions, or economic conditions. Consideration of these external factors is essential for a holistic understanding of the store's performance.




