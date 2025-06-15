# AdventureWorks Dataset Analysis

## Introduction
This repository showcases data visualization skills using **Microsoft Azure** to create interactive dashboards based on the **AdventureWorks dataset**. The analysis focuses on extracting meaningful insights from sales and product data.

## Dataset Overview
The AdventureWorks dataset includes multiple tables related to:
- **Products**
- **Sales**
- **Customers**
- **Geographical Information**
- **Order Details**

This dataset provides a strong foundation for data visualization and trend analysis.

## Data Extraction
The following **SQL query** is used to retrieve relevant product and category information:

```sql
SELECT p.ProductID, p.Name AS ProductName,
       c.Name AS Category, p.ListPrice
FROM SalesLT.Product AS p
JOIN SalesLT.ProductCategory AS c
ON p.ProductCategoryID = c.ProductCategoryID;
