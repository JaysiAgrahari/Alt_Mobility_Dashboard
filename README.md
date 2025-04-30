# Alt_Mobility_Dashboard
Customer Retention Analysis Project

Overview
This project analyzes customer retention using cohort analysis. It includes SQL queries for data transformation and a Power BI dashboard for visualizing customer retention trends.

Datasets Used

customer_orders.csv — contains customer purchase records with order dates.

payments.csv — includes payment success/failure status for each order.

Approach

Data Preparation (SQL/Python)

Loaded and cleaned data from CSV files.

Derived CohortMonth: the month of a customer's first purchase.

Created OrderMonth from each order date.

Calculated CohortIndex: number of months since the first purchase.

Counted unique customers per (CohortMonth, CohortIndex) pair.

Calculated Retention % by dividing retained customers by initial cohort size.

Visualization in Power BI

Imported processed data into Power BI.

Built:

Line Chart: Retention trend per cohort over months.

Bar Chart: Retention % comparison between cohorts.

Filters: Cohort selection, retention window, etc.

Provided DAX formulas to transform and format date fields.

Key Metrics

Cohort Size: Total customers in each first-month group.

Customer Retention %: Share of retained users across future months.

Payment Success Rate

How to Use

Open customer_retention_dashboard.csv in Power BI.

Use slicers and charts to explore cohort behaviors.


