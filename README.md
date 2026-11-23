BUSINESS SALES DATA ANALYSIS

Future Interns – Data Science & Analytics Internship | Task

Project Overview
This project analyzes business sales data to understand revenue performance over time, identify products generating the most revenue, compare sales across product categories, and evaluate regional performance. A Power BI dashboard presents key performance indicators (KPIs) and visual comparisons in an easy-to-understand format.

![image alt] (https://github.com/gbvijayakumar-svg/FUTURE_DS_01/blob/90956f6baea8be8028bf933bff4f96526f21a14b/Screenshot%202026-11-23%20183742.png)

Internship: Future Interns – Data Science & Analytics Internship
Task: Task 1 – Business Sales Data Analysis
Primary Tool: Microsoft Power BI Desktop
Supporting Features: Power Query and DAX
Project Objectives
Inspect and prepare the sales dataset for analysis.
Calculate total revenue, distinct orders, and total quantity sold.
Study monthly revenue trends.
Identify the top 10 products by revenue.
Compare revenue by product category.
Compare revenue across regions.
Build an interactive dashboard to communicate findings.
Dataset Description
The dataset is a CSV file named FUTURE_DS_01_Task1_Sales_Data.csv. It contains 56 sample sales records.

Column	Meaning
Order ID	Identifier for an order; used to count distinct orders.
Order Date	Date on which the order was placed.
Ship Date	Date on which the order was shipped.
Region	Sales region associated with the record.
Category	Main product category.
Sub-Category	More specific product grouping.
Product Name	Name of the product.
Quantity	Number of units sold.
Unit Price	Price per unit.
Sales	Revenue value recorded for the sales row.
Profit	Profit value recorded for the sales row.
Tools and Technologies
Microsoft Power BI Desktop: Used to import data, create measures, build charts, and design the dashboard.
Power Query Editor: Used to access and inspect the dataset before loading it.
DAX: Used to define calculations for the KPI cards and charts.
CSV: Source file format for the sales data.
Data Import Process

Opened Power BI Desktop.

Selected Home → Get Data → Text/CSV.

Selected FUTURE_DS_01_Task1_Sales_Data.csv.

Selected Transform Data to inspect the dataset in Power Query Editor.

Selected Close & Apply to load the data into Power BI.

Data Cleaning and Preparation

The dataset was inspected before analysis. The following checks should only be described as completed if they were actually performed.

Column names: Checked that fields had understandable names.
Data types: Checked date, numeric, and text columns.
Missing values: Checked important fields for blanks.
Duplicate records: Reviewed possible duplicate rows. Repeated Order IDs are not automatically duplicates.
Date validity: Checked date interpretation and shipping dates.
Numeric validity: Checked numeric fields such as Quantity, Unit Price, Sales, and Profit.
Consistency: Reviewed Region and Category labels.
Sales Data: Imported the existing Sales values and used them to calculate total revenue.
DAX Measures
The following measures were created in Power BI.

Total Revenue

Total Revenue = SUM('FUTURE_DS_01_Task1_Sales_Data'[Sales])
Adds the Sales values to calculate overall revenue.

Total Orders

Total Orders = DISTINCTCOUNT('FUTURE_DS_01_Task1_Sales_Data'[Order ID])
Counts unique Order IDs.

Total Quantity

Total Quantity = SUM('FUTURE_DS_01_Task1_Sales_Data'[Quantity])
Adds the Quantity values to calculate total units sold.

KPI Results
The following values were observed in the Power BI report.

KPI	Result
Total Revenue	15,132.75
Total Orders	56
Total Quantity	249
Total Profit	Approximately 2.47K
These values describe the sample dataset used in this project.

Dashboard Visualizations
9.1 KPI Cards Created Card visuals for Total Revenue, Total Orders, and Total Quantity. These cards provide a quick summary of key sales figures.

9.2 Monthly Revenue Trend Created a line chart with Order Date on the X-axis and Total Revenue on the Y-axis. Adjusted the date hierarchy to display monthly revenue values.

9.3 Top 10 Products by Revenue Created a bar chart with Product Name as the category and Total Revenue as the value. Sorted it by revenue in descending order and applied a Top N filter to display the 10 highest-revenue products.

9.4 Revenue by Product Category Created a clustered column chart with Category on the X-axis and Total Revenue on the Y-axis. Each category is displayed as a separate bar.

9.5 Revenue by Region Created a clustered bar chart with Region on the Y-axis and Total Revenue on the X-axis to compare regional sales performance.

Validation and Quality Checks
Checked that Total Revenue matches the sum of the Sales column.
Verified that Total Orders uses DISTINCTCOUNT on Order ID.
Verified that Total Quantity sums the Quantity column.
Checked that the monthly chart displays multiple month-level data points.
Checked that the Top 10 Products chart contains no more than 10 products and is sorted from highest to lowest revenue.
Checked that each product category appears separately.
Checked that the region chart displays the available regions.
Saved and reopened the Power BI report to check that it loads correctly.
Conclusion
This project demonstrates a basic business analytics workflow, including importing data, preparing data, creating KPI measures, visualizing monthly revenue, and comparing product, category, and regional performance. The Power BI dashboard presents key sales information in a visual format, making it easier to understand the data.
