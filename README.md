# Retail Sales Analysis Dashboard

## SQL and Power BI Project for Business Insights & Data Visualization

## Alternative Professional Titles :

•Retail Sales Data Analysis using SQL & Power BI

•Business Sales Dashboard Project

•Customer & Revenue Analysis Dashboard

•Retail Business Intelligence Dashboard

•Sales Performance Analysis using SQL & Power BI

## 1. Which product category generates the highest revenue?

```SELECT Product_Category, SUM(Total_Amount) AS

Total_Revenue

FROM retail_sales

GROUP BY Product_Category

ORDER BY Total_Revenue DESC;
```
### Insight:
Electronics was the top-performing product category by revenue.

## 2. Which month has the highest sales?
```SELECT MONTH(Date) AS Month,
       SUM(Total_Amount) AS Total_Sales
FROM retail_sales
GROUP BY MONTH(Date)
ORDER BY Total_Sales DESC; 
```

## 3. Which gender contributes more to total sales?
```SELECT Gender,
       SUM(Total_Amount) AS Total_Sales
FROM retail_sales
GROUP BY Gender;
```

## 4. What is the average spending per customer?
```SELECT Customer_ID,
       AVG(Total_Amount) AS Avg_Spending
FROM retail_sales
GROUP BY Customer_ID
ORDER BY Avg_Spending DESC;
```

## 5. Which age group purchases the most?
```SELECT
CASE
    WHEN Age BETWEEN 18 AND 25 THEN '18-25'
    WHEN Age BETWEEN 26 AND 35 THEN '26-35'
    WHEN Age BETWEEN 36 AND 45 THEN '36-45'
    ELSE '46+'
END AS Age_Group,
SUM(Total_Amount) AS Total_Sales
FROM retail_sales
GROUP BY Age_Group
ORDER BY Total_Sales DESC;
```

## 6. Which customers are top spenders?
```SELECT Customer_ID,
       SUM(Total_Amount) AS Total_Spending
FROM retail_sales
GROUP BY Customer_ID
ORDER BY Total_Spending DESC
LIMIT 10;
```

## 7. What is the total quantity sold by category?
```SELECT Product_Category,
       SUM(Quantity) AS Total_Quantity_Sold
FROM retail_sales
GROUP BY Product_Category
ORDER BY Total_Quantity_Sold DESC;
```

## 8. What is the daily sales trend?
```SELECT Date,
       SUM(Total_Amount) AS Daily_Sales
FROM retail_sales
GROUP BY Date
ORDER BY Date;
```

## 9. Which product category has the highest average transaction value?
```SELECT Product_Category,
       AVG(Total_Amount) AS Avg_Transaction_Value
FROM retail_sales
GROUP BY Product_Category
ORDER BY Avg_Transaction_Value DESC;
```

## 10. What is the total revenue generated?
```SELECT SUM(Total_Amount) AS Total_Revenue
FROM retail_sales;
```

## Power BI Dashboard Questions & KPIs
KPI Cards
Total Revenue
Total Orders
Total Quantity Sold
Average Order Value
Total Customers

## Dashboard Visualizations
1. Sales by Product Category
Business Insight
Shows which category contributes the most revenue.

## 2. Monthly Sales Trend
Business Insight
Tracks sales performance over time and identifies peak months.

## 3. Sales by Gender
Business Insight
Shows customer demographic contribution.

## 4. Sales by Age Group
Business Insight
Identifies the most profitable customer age segment.

## 5. Top 10 Customers
Business Insight
Highlights loyal and high-value customers.

## 6. Quantity Sold by Category
Business Insight
Analyzes product demand and inventory requirements.

## 7. Daily Sales Trend
Business Insight
Shows sales fluctuations and customer buying behavior.

## Final Project Conclusion
This project demonstrates practical data analyst skills by combining SQL analysis with Power BI dashboard visualization. It provides valuable business insights into customer behavior, product performance, and sales trends. The project showcases the ability to transform raw data into actionable business intelligence.
