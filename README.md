# Sales-Performance-Dashboard-PowerBI

## Table of Contents
- [1. Introduction](#1-introduction)
- [2. Specifications](#2-specifications)
- [3. KPIs](#3-kpis)
- [4. Modeling](#4-modeling)
- [5. Dashboard](#5-dashboard)
- [6. Lessons Learned](#6-lessons-learned)

## 1. Introduction

The objective of this project is to model, measure, analyze, and track the sales performance within a retail store. The project leverages the Orders, People, and Returns datasets to extract valuable insights on sales and order trends. By utilizing predefined dimensions and key performance indicators (KPIs), three distinct analyses are generated to cater to the informational needs of various stakeholders.

## 2. Specifications

This analysis covers key measures including:
- **Cost of Goods Sold (COGS)**
- **Year-over-Year Sales Growth by Order Date**
- **Sales Amount Discounted**
- **Consumer Sales**
- **Amount Returned**
- **Rolling 4-Month Sales by Order Date**
- **Last Data Model Refresh**
- **Total Sales by Month Ordered and Month Shipped**

The dashboard comprises three pages:
1. **Sales Summary:** Tailored for the executive team, providing a high-level overview of year-over-year sales and gross margin performance, segmented by product category, customer segment, time period, and region. Key performance indicators include sales amount, gross margin, and cost.
   
2. **Product Detail:** Designed for the sales and marketing teams to gain insights into individual product performance, aiding in refining operational strategies and targeted campaigns.
   
3. **Customer Detail:** Created for the CRM and marketing campaign departments, this page offers insights into customer behaviors, utilizing top N analysis to identify the most valuable customers and analyzing each customer segment's contribution to total sales.

## 3. KPIs

The dataset consists of 9 tables, including 3 source data tables and 6 data mart tables:

- **Orders:** The fact table containing customer code, order code, order date, postal code, last product update, and product code.
- **People:** Contains information about customers and regions.
- **Returns:** Tracks data on order codes and whether products have been returned.
- **Calendar:** Provides a single record for each date used in the analysis.
- **Customer:** Generated from the Orders table, detailing customer code, customer name, and segment.
- **Date Type:** Specifies whether the date is an order date or a ship date.
- **Last Refresh:** Updates each time the dashboard is refreshed, recording the latest refresh time.
- **Product:** Generated from the Orders table, detailing product code, category, sub-category, product name, and last product update.
- **Region:** Contains postal code, country, state, city, and region information, generated from the Orders table.

## 4. Modeling

The data modeling process involved structuring the tables to support accurate and efficient analysis. Below is a visual representation of the data model:

![Data Modeling Workflow](https://github.com/user-attachments/assets/5c655221-fb2f-4d9a-8a91-c367094b12f8)

## 5. Dashboard

The Power BI dashboard visualizes the data, enabling stakeholders to interpret the analysis effectively. *(Note: All data has been replaced with simulated data.)*

![Dashboard Example](https://github.com/user-attachments/assets/9574ed59-162d-46b2-b2a9-757cf6082a94)

## 6. Lessons Learned

1. **Gross Margin Rate as a Profitability Metric:**  
   The Gross Margin Rate was crucial in understanding product profitability. Focusing on high-margin products helped maximize overall revenue.

2. **Comprehensive Trend Analysis:**  
   Analyzing both short-term (rolling 4-month) and long-term (year-over-year) trends provided valuable insights. This dual analysis optimized inventory management and established performance benchmarks, addressing both immediate and long-term market dynamics.

3. **Return Rate as a Key Performance Indicator:**  
   Monitoring the Return Rate allowed the product team to identify areas for improvement. By addressing the causes of returns, the project improved product quality and customer satisfaction, ultimately enhancing profitability.
