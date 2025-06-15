# AdventureWorks Dataset Analysis:
![azure lab1](https://github.com/user-attachments/assets/26ca115a-0b5b-419f-b8d7-09f71b4a66e0)

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
Results
Sample results extracted from the dataset:

ProductID	Product Name	Category	List Price
788	Mountain-300 Black, 48	Mountain Bikes	1079.99
980	Mountain-400-W Silver, 38	Mountain Bikes	769.49
981	Mountain-400-W Silver, 40	Mountain Bikes	769.49
985	Mountain-500 Silver, 40	Mountain Bikes	564.99
Data Visualization & Dashboard Insights
Using Microsoft Azure, various dashboards have been created to visualize key insights, including:

Sales Performance: Analyzing sales trends by product category.

Price Distribution: Identifying pricing patterns across different product lines.

Customer Demographics: Understanding purchase behavior across customer segments.

Monthly Trends: Visualizing fluctuations in sales over time.

Technologies Used
Microsoft Azure: SQL Database, Query Editor, and Dashboarding Tools.
Conclusion:
This project demonstrates strong data visualization expertise using Microsoft Azure to generate insights from the AdventureWorks dataset. The dashboards provide a clear view of trends, enabling data-driven decision-making.v
# Microsoft Azure Data Visualization Project

## Overview
This repository showcases **data visualization skills** using **Microsoft Azure** to create an interactive dashboard based on a structured dataset.

## Dataset Description
![azure lab2](https://github.com/user-attachments/assets/308a82de-3f84-4b87-8c70-1ca150eef7e8)

The dataset is stored in **Microsoft Azure Storage Tables** and contains **product information** with the following attributes:
- **RowKey**: A unique identifier for each item.
- **Timestamp**: The time when the data was recorded.
- **Name**: The product name.
- **Price**: The cost of each product.

### Sample Data
| RowKey | Timestamp                  | Name    | Price |
|--------|----------------------------|---------|-------|
| 1      | 2024-03-31T10:05:34.50...  | Widget  | 2.99  |
| 2      | 2024-03-31T10:06:46.54...  | Kniknak | 1.99  |

## Data Visualization with Microsoft Azure
Leveraging **Microsoft Azure**, this project highlights **dashboard creation** to transform raw data into meaningful insights.

### Visualization Highlights:
- **Price Distribution**: Analyzing pricing trends across different product categories.
- **Timestamp-based Patterns**: Identifying purchase behaviors over time.
- **Interactive Filters**: Enhancing user exploration of product information.

## Technologies Used
- **Microsoft Azure Storage Tables**: Hosting and managing dataset.
- ## Insights & Outcomes
The dashboard provides **actionable insights**, enabling data-driven decisions through **clear, interactive visualizations**.
# Taxi Rides Data Analysis

## Overview
This repository presents an analysis of taxi ride data, utilizing **Microsoft Azure** for data processing and visualization. The project focuses on understanding trip patterns, including **average distances traveled per day of the week**.

## Dataset Description
![Screenshot 2025-06-01 202207](https://github.com/user-attachments/assets/9dc01134-1f42-4cac-be31-699b0a50712b)


The dataset captures key details of taxi rides, including:
- **Pickup Date & Time**: Timestamp of ride initiation.
- **Trip Distance**: Total distance covered per trip.
- **Day of the Week**: Extracted from timestamps for trend analysis.

### Sample Data
| Day       | AvgDistance          |
|-----------|----------------------|
| Thursday  | 2.86                 |
| Wednesday | 2.83                 |
| Tuesday   | 2.82                 |
| Saturday  | 2.99                 |
| Friday    | 2.85                 |
| Monday    | 2.88                 |
| Sunday    | 3.08                 |

## Data Processing with SQL
The following **SQL query** was executed in **Microsoft Azure** to extract meaningful insights:

```sql
SELECT DATENAME(dw, lpepPickupDatetime) AS Day,
       AVG(tripDistance) AS AvgDistance
FROM "taxi-rides"
GROUP BY DATENAME(dw, lpepPickupDatetime);
This query calculates the average trip distance for each day of the week, enabling a deeper understanding of taxi ride trends.

Dashboard Insights
Using Microsoft Azure, an interactive dashboard has been created to visualize key insights:

Trend Analysis: Average trip distances across different days.

Ride Distribution: Breakdown of taxi activity across the week.

Comparative Metrics: Identifying peak travel days.

Technologies Used
Microsoft Azure SQL Database: Storing and processing taxi ride data.

Azure Fabric Dashboards: Creating interactive visualizations.

SQL Querying: Filtering and analyzing ride metrics.

Conclusion
This project demonstrates data visualization expertise using Microsoft Azure, transforming raw taxi ride data into actionable insights. The interactive dashboard helps analyze trends and optimize decision-making.
# Taxi Rides Data Visualization

## Overview
This project demonstrates **data visualization skills** using **Microsoft Azure** to analyze taxi ride trends. The dataset captures passenger count variations over time, offering insights into demand patterns.

## Dataset Details
The dataset includes:
- **Pickup Date & Time** (`lpepPickupDatetime`)
- **Passenger Count** (`Sum of passengerCount`)
- **Geographical Data** (Pickup & Dropoff locations)
- **Fare Details** (Total fare, tip amount, tolls)

### Sample Data
| Date          | Passenger Count |
|--------------|----------------|
| 2010-05-12   | 245            |
| 2011-07-08   | 290            |
| 2014-03-15   | 315            |
| 2016-09-22   | 198            |
| 2020-11-30   | 220            |

## Data Visualization & Dashboard Insights
Using **Microsoft Azure**, a **line chart** was created to analyze **passenger count trends** over time. Key insights:
- **Peak Demand Periods**: Identifying fluctuations in taxi ride usage.
- **Long-Term Trends**: Understanding how demand has evolved across years.
- **Interactive Data Filters**: Enhancing exploratory analysis.

## Technologies Used
- **Microsoft Azure SQL Database**: Data storage and processing.
- **Azure Dashboard**: Visualizing passenger count trends.
- **SQL Querying**: Extracting structured insights.

## Conclusion
This project highlights **data visualization expertise** using **Microsoft Azure**, transforming taxi ride records into actionable insights. The interactive dashboard facilitates trend analysis for optimized decision-making.

## Contact
For inquiries or collaboration, reach out via **[Your Email]** or **[LinkedIn Profile]**.
# Taxi Data Analysis with Microsoft Azure

## Overview
This repository presents an analysis of **taxi ride data**, leveraging **Microsoft Azure** to create an interactive dashboard for data visualization.

## Dataset Description
The dataset contains **taxi trip details**, including:
- **VendorID**: Identifies the taxi provider.
- **Pickup & Dropoff Datetime**: Timestamp for the trip start and end.
- **Passenger Count**: Number of passengers per trip.
- **Trip Distance**: Total miles covered in each ride.
- **RatecodeID**: Rate classification for the fare.
- **Store & Forward Flag**: Indicates if the trip data was temporarily stored before transmission.

### Sample Data
| VendorID | Pickup Datetime | Dropoff Datetime | Passenger Count | Trip Distance |
|----------|----------------|------------------|-----------------|---------------|
| 2        | 2022-06-01 00:28:57 | 2022-06-01 00:28:30 | 1 | 1.35 |
| 2        | 2022-06-01 00:33:11 | 2022-06-01 00:31:52 | 5 | 0.89 |
| 2        | 2022-06-01 00:35:31 | 2022-06-01 00:14:57 | 1 | 5.0 |
| 2        | 2022-06-01 00:13:05 | 2022-06-01 00:11:11 | 2 | 0.85 |
| 2        | 2022-06-01 00:24:00 | 2022-06-01 00:20:04 | 2 | 2.3 |

## Data Visualization & Dashboard Features
Using **Microsoft Azure**, this project includes a **real-time streaming dashboard** that visualizes taxi ride trends.

### Key Insights:
- **Trip Distance Trends**: Understanding how trip lengths vary across different vendors.
- **Passenger Count Analysis**: Identifying ride-sharing behaviors.
- **Interactive Data Processing**: Transforming events and destinations dynamically.

## Technologies Used
- **Microsoft Azure**: Hosting, streaming, and processing data.
- **Azure Fabric Dashboards**: Building interactive visualizations.
- **SQL Querying**: Filtering and analyzing taxi ride data.

## Conclusion
This project highlights strong **data visualization expertise** using **Microsoft Azure**, transforming taxi ride data into actionable insights.

## Contact
For collaboration or inquiries, reach out via **[Your Email]** or **[LinkedIn Profile]**.








