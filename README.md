Insight Reporting - Kelly and Dyre
Overview
This project delivers a streamlined data reporting and analytics solution for Kelly and Dyre by integrating CSV data ingestion, SQL-based normalization, and Power BI for dashboard creation. The goal is to enable efficient and actionable insights from raw operational data, enhancing the client’s decision-making capacity.

📁 Data Sources
CSV Files
Multiple raw CSV files are provided by the client (e.g., sales_data.csv, customer_info.csv, transactions.csv). These files contain unstructured or semi-structured data that require transformation before analysis.

🛠 Data Normalization (SQL)
Using SQL Server, we normalize the ingested data into a relational schema that supports:

Elimination of Redundancy: Repeating groups and non-atomic fields are decomposed.

Referential Integrity: Foreign keys and indexed relationships are used to link tables like Customers, Sales, Products, and Regions.

Data Cleansing: SQL scripts handle null values, inconsistent formatting, and duplicates.

Key tables created:

dbo.Customers

dbo.Products

dbo.Sales

dbo.Regions

🔍 Stored Procedures are included to automate the transformation pipeline from raw CSV import to staging and normalized tables.

📈 Visualization (Power BI)
Power BI dashboards have been built to reflect:

Sales Trends (by product, region, and time)

Customer Segmentation

Performance KPIs

Revenue Heatmaps

Interactive features:

Drill-through by region or product

Dynamic filtering by time period

Real-time refresh (if connected to live SQL source)

⚙️ Workflow Summary
CSV Import → Raw data is loaded into SQL staging tables.

SQL Normalization → Data is transformed and structured using scripts.

Data Model → Normalized tables are imported into Power BI using relationships.

Visualization → Reports and dashboards are designed to support business decisions.

📝 Deliverables
README.md (this file)

Normalization SQL scripts (/sql/normalization_scripts.sql)

Power BI report file (/reports/KellyAndDyre_Insights.pbix)

Data model documentation (/docs/data_model.pdf)

🔐 Notes
Ensure all data files are placed in the /data folder before running SQL import scripts.

SQL scripts are designed for Microsoft SQL Server 2019+.

Power BI Desktop (Version 2.125+) is recommended for full compatibility.

