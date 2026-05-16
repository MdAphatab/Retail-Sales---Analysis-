# Retail Sales Analysis Dashboard

## SQL and Power BI Project for Business Insights & Data Visualization

## Alternative Professional Titles :

•Retail Sales Data Analysis using SQL & Power BI

•Business Sales Dashboard Project

•Customer & Revenue Analysis Dashboard

•Retail Business Intelligence Dashboard

•Sales Performance Analysis using SQL & Power BI

## 1. Which product category generates the highest revenue?

```SQL

SELECT Product_Category, SUM(Total_Amount) AS

Total_Revenue

FROM retail_sales

GROUP BY Product_Category

ORDER BY Total_Revenue DESC;
```
### Insight 
Electronics was the top-performing product category by revenue.

