Vendor Performance Data Analytics
This project delivers a full-cycle vendor performance analysis for the Retail and Wholesale industry, integrating ETL, statistical analysis, and interactive visualization to optimize inventory, sales, and vendor strategies.

Objective:
To maximize profitability by analyzing vendor performance, inventory efficiency, and sales patterns, providing actionable insights for strategic decision-making.

Business Problem:

Inefficient pricing strategies affecting margins.

Poor inventory turnover leading to capital being tied up.

High vendor dependency posing supply risks.

Data Sources & Scale:

Multiple CSV files: Purchase, Sales, Vendor Invoice, Inventory.

Sales table: >10 million records.

Aggregated dataset: 10,692 records ready for analytics and visualization.

Technical Environment & Tools:

Data Storage & Querying: SQLite and SQL for storing large CSVs, performing complex joins, and optimizing queries.

ETL & Scripting: Python (Pandas, SQLAlchemy, OS, Time, Logging) for automated data ingestion, cleaning, transformation, and feature engineering.

Advanced Analysis & Statistics: Python (Matplotlib, Seaborn, SciPy) for exploratory data analysis, outlier detection, correlation analysis, and statistical validation.

Reporting & Visualization: Power BI for creating interactive dashboards, KPIs, custom charts, and actionable business insights.

Methodology
1. Data Ingestion (ETL Pipeline)

Database Setup: Imported raw CSV files into SQLite using Python.

Automation & Scripting: Built ingestion_db.py for reusable ETL operations.

Logging & Monitoring: Implemented logging to track execution time, errors, and workflow completion.

Performance Consideration: Optimized insertion of large datasets (~10M rows) to prevent runtime errors.

2. Data Aggregation & SQL Optimization

Performed initial EDA using SQL to understand table relationships.

Created aggregated summary tables combining sales, purchase, and invoice data.

Optimized joins to reduce query execution from >8 minutes to <1 minute.

Persisted aggregated tables in the database for faster downstream analysis.

3. Data Cleaning & Feature Engineering

Imputed missing values for sales/quantity with zero.

Standardized categorical fields (e.g., vendor names) by trimming whitespace.

Created key analytical features:

Gross Profit

Profit Margin (%)

Stock Turnover

Sales-to-Purchase Ratio

Unsold Inventory Value (capital locked in unsold stock).

4. Advanced Analysis & Statistical Validation

Conducted detailed EDA on the aggregated dataset using histograms, boxplots, and heatmaps.

Correlation analysis revealed relationships between profit margin, sales, and vendor performance.

Targeted insights extracted:

198 brands with low sales but high margins requiring promotional intervention.

Top 10 vendors contributing 65.69% of purchase dollars.

Capital locked in unsold inventory quantified at $2.7M.

Bulk orders reduce unit costs by ~72%, validating bulk pricing strategies.

Statistical validation:

95% Confidence Intervals for profit margins.

T-Test confirming significant difference between top-performing and low-performing vendors.

5. Dashboarding & Reporting

Developed a Power BI dashboard with:

KPIs: Total Sales, Gross Profit, Unsold Capital.

Donut/Parito Charts: Purchase Contribution by Vendor.

Funnel charts: Low-turnover vendors.

Scatter plots: Target brands for sales promotion.

DAX Calculations: Implemented advanced measures and calculated tables within Power BI.

Compiled a final report with methodology, visualizations, and actionable insights for business strategy and cost optimization.

Key Achievements & Outcomes

Designed a full ETL pipeline capable of handling multi-million row datasets.

Created a fast, optimized aggregated dataset to streamline analysis.

Built an interactive dashboard enabling stakeholders to explore vendor performance dynamically.

Provided data-driven recommendations for inventory and pricing strategies, improving operational decision-making.
