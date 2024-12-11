# End2End Analysis

This repository contains advanced SQL use cases and projects across domains like **Finance Analytics**, **Supply Chain Analytics**, and **Top Customers, Products, and Markets Analysis**. These projects demonstrate robust SQL implementations, including the use of user-defined functions, stored procedures, triggers, events, CTEs, and optimization techniques.

## Project Overview

### 1. **Finance Analytics**
- Implemented user-defined functions to calculate fiscal years and optimized sales queries using these functions.
- Generated detailed gross sales reports and monthly gross sales summaries.
- Created stored procedures for:
  - Automating monthly gross sales reports for specific customers.
  - Assigning market badges (Gold or Silver) based on performance.
  
[View Finance Analytics SQL File](https://github.com/Ranjith-Senthilkumar/MYSQL-Queries/blob/main/Financials_Query)

### 2. **Supply Chain Analytics**
- Designed helper tables (`fact_act_est`) for actual and forecasted quantities using `LEFT JOIN` and `UNION`.
- Developed triggers to automate updates to helper tables upon data insertion in sales and forecast tables.
- Scheduled database events to manage periodic log purges and cleanup operations.
- Calculated forecast accuracy reports using temporary tables and CTEs.

[View Supply Chain Analytics SQL File](https://github.com/Ranjith-Senthilkumar/MYSQL-Queries/blob/main/Supply_chain_analysis_query)

### 3. **Top Customers, Products, and Markets Analysis**
- Generated pre-invoice and post-invoice discount reports using views and CTEs.
- Developed stored procedures to identify:
  - Top markets by net sales.
  - Top customers in specific markets and fiscal years.
- Employed window functions (`ROW_NUMBER`, `RANK`, `DENSE_RANK`) to rank expenses and product performance across divisions.

[View Top Customers, Products, and Markets SQL File](https://github.com/Ranjith-Senthilkumar/MYSQL-Queries/blob/main/Top%20and%20Bottom%20N%20queries)

## Key Features

### Data Definition Language (DDL):
- Created tables, views, and indexes for efficient data storage and retrieval.
- Designed triggers for automated data manipulation and integrity.

### Data Manipulation Language (DML):
- Performed complex joins, inserts, updates, and deletions.
- Wrote dynamic stored procedures and events for repetitive tasks.

### Optimization:
- Avoided function calls in queries by redesigning tables with pre-calculated columns.
- Used indexes to enhance query performance for large datasets.

## Usage

### Run SQL Scripts:
- Execute the provided SQL scripts in MySQL Workbench or any compatible SQL client.
- Scripts include DDL, DML, and examples of function, procedure, trigger, and event usage.

### Query Examples:
- **Top customers and markets analysis**: Use `get_top_n_markets_by_net_sales` and `get_top_n_customers_by_net_sales` procedures.
- **Forecast accuracy reports**: Use CTEs or `get_forecast_accuracy` procedure for fiscal year-specific insights.

### Automation:
- Utilize triggers for real-time data updates.
- Schedule periodic tasks with database events.

## About
These projects were created to solve real-world analytical problems across multiple domains using advanced SQL features. I designed and executed various DDL and DML statements in MySQL to manage and analyze data effectively.
