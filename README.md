# PowerBI-Sales-Performance-Dashboard
## Table of Contents
- [1.Introduction](#1Introduction)
- [2.Specifications](#2Specifications)
- [3.KPIs](#3KPIs)
- [4.Modeling](#4Modeling)
- [5.Dashboard](#5Results)
- [6.Lesson Learned](#6Lesson-Learned)
## 1.Introduction
The object of this solution delivery is to model, measure, analyze and track the status of sales within one retail store. To achieve this, the Orders, People, and Returns datasets have been made accessible to extract valuable insights on sales and orders. Additionally, by employing predefined dimensions and key performance indicators, three different analysis will be generated, serving the information needs of various stakeholders.
## 2.Specifications
The analysis should encompass key measures such as the cost of goods sold, year-over-year sales growth by order date, sales amount discounted, consumer sales, amount returned, rolling 4-month sales by order date, the last refresh of the data model, and total sales by both month ordered and month shipped.

The dashboard is composed of three pages: Sales Summary, Product Detail, and Customer Detail. The Sales Summary page is designed for the executive team, providing a high-level overview of year-over-year sales and gross margin performance trends compared to the previous year, segmented by product category, customer segment, time period, and region. Potential key performance indicators include sales amount, gross margin, and cost.

The Product Detail page aims to assist the sales and marketing teams in gaining a deeper understanding of individual product performance, enabling them to refine operational strategies and deliver targeted campaigns.

Lastly, the Customer Detail page is tailored for the CRM and marketing campaign department, offering insights into customer behaviors. It utilizes top N analysis to identify the most valuable customers and examines the contribution of each customer segment to the total sales amount.
## 3.KPIs
The dataset consists of a total of 9 tables, including 3 source data tables and 6 data mart tables.

**Orders:** This fact table contains information such as customer code, order code, order date, postal code, last product update, and product code

**People:** Provides information about person (cutomer name) and regions

**Returns:** Contains data on order codes and indicates whether a product has been returned

**Calender:** Includes a single record for each date used in the analysis

**Customer:** Generated from the order table, it includes details such as customer code, customer name, and segment

**Date Type:** Specifies the type of date, either order date or ship date

**Last Refresh:** Each time the dashboard is refreshed, this table updates and returns the latest refresh time

**Product:** Generated from the order table with a predefined filter, it includes product details such as product code, category, sub-category, product name, and last product update

**Region:** Generated from the order table, this table contains information about postal code, country, state, city, and region
## 4.Modeling 
![20240811032926](https://github.com/user-attachments/assets/5c655221-fb2f-4d9a-8a91-c367094b12f8)
## 5.Dashboard
![20240811033042](https://github.com/user-attachments/assets/9574ed59-162d-46b2-b2a9-757cf6082a94)
## 6.Lesson Learned
**1.Gross Margin Rate as a Profitability Metric:**
The Gross Margin Rate proved vital in understanding product profitability. By focusing on high-margin products, the project effectively contributed to maximizing overall revenue.

**2.Comprehensive Trend Analysis:**
Analyzing both short-term (rolling 4-month) and long-term (year-over-year) trends provided valuable insights. This dual analysis optimized inventory management and established performance benchmarks, enabling the project to address both immediate and long-term market dynamics.

**3.Return Rate as a Key Performance Indicator:**
Monitoring the Return Rate helped the product team identify areas for improvement. By addressing the causes of returns, the project improved product quality and customer satisfaction, thereby enhancing profitability.
