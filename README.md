# Amazon-Sales-Intelligence-Dashboard-Excel
Business intelligence dashboard built in Excel to analyze retail sales performance, delivery efficiency, and cancellation trends using Pivot Tables and advanced Excel functions.

🧭 # Project Background

Retail companies generate large volumes of transactional data every day. However, raw sales data alone rarely provides actionable insights for decision-makers.

Imagine you are a Business/Data Analyst at an Amazon retail partner company. The sales team shares a dataset containing 100 sales transactions across different regions, products, and customers, but leadership struggles to understand:

Which regions are generating the most revenue

Which products are driving sales performance

How efficient the delivery process is

Where cancellations are occurring and why

Your task is to transform raw operational data into a decision-support dashboard that enables management to quickly identify trends, monitor KPIs, and make smarter business decisions.

🎯 Project Goal

Build a dynamic Excel dashboard that converts raw transaction data into clear insights and performance indicators for business stakeholders.

The dashboard enables users to:

✔ Monitor revenue performance across regions
✔ Identify top-performing product categories
✔ Track delivery efficiency
✔ Detect regional cancellation issues
✔ Explore insights interactively using filters

🗂 Dataset Overview

The dataset simulates Amazon retail sales transactions including:

Column	Description
Order Date	Date when the order was placed
Delivery Date	Date when the order was delivered
Cancel Date	Date of order cancellation
Region	Sales region
Product Category	Product classification
Customer ID	Unique customer identifier
Sales Amount	Transaction revenue
Payment Method	Payment mode used
Delivery Status	Order completion status

Total Records: 100 transactions

🔎 Analytical Approach

The analysis followed a structured data analytics workflow similar to real-world projects:

1️⃣ Data Cleaning & Preparation

Before performing analysis, the dataset required preparation:

Converted text dates into proper date formats

Removed inconsistent spacing and formatting

Standardized Region, Payment Method, and Delivery Status

Identified cancelled orders using Cancel Date

This step ensured the dataset was accurate and analysis-ready.

2️⃣ Data Enrichment using XLOOKUP

To simulate real-world relational data, a Customer Master dataset was created.

Using XLOOKUP, Customer IDs were matched to Customer Names.

Example formula:

=XLOOKUP(Customer_ID, Customer_Master[Customer_ID], Customer_Master[Customer_Name])

This allowed the dataset to become more informative and business-ready.

3️⃣ Delivery Performance Analysis

To evaluate logistics efficiency, delivery speed was categorized:

=IF(Delivery_Date - Order_Date <= 2,"Fast","Slow")

This enabled tracking of fast vs slow deliveries across regions.

Cancelled orders were handled using IFERROR to avoid calculation errors.

4️⃣ Pivot Table Insights

Pivot tables were used to summarize business performance:

📊 Revenue by Region and Product Category
📊 Order Count by Delivery Status
📊 Average Delivery Time

Average Delivery Time was calculated as:

Delivery Date – Order Date

Pivot filters allow stakeholders to explore data dynamically.

📈 Key Business KPIs

The dashboard highlights important metrics used in retail performance monitoring.

💰 Total Revenue

Total sales value generated from all transactions.

⚡ Fast Delivery Rate

Percentage of orders delivered within 2 days.

🏆 Top Performing Regions

Regions contributing the highest sales revenue.

📦 Highest Selling Product Category

Product category generating the most revenue.

❌ Cancellation Rate

Cancellation rate was calculated using:

Cancelled Orders / Total Orders

This metric helps identify operational or logistical problems in specific regions.

📊 Dashboard Design

The final dashboard presents insights in a clean and interactive format.

Dashboard Components

Filters (Slicers)

Region

Payment Method

Delivery Status

Month

Visualizations

Revenue by Region

Sales by Product Category

Delivery Status Distribution

KPI Performance Cards

Layout Structure
Left Section → Interactive Filters  
Center Section → Charts & Visual Analysis  
Right Section → KPI Cards

This layout ensures decision-makers can quickly understand business performance.

💡 Business Insights Generated

Through the analysis, several insights emerged:

✔ Certain regions consistently generate higher revenue contributions

✔ Delivery efficiency varies significantly across regions

✔ Some product categories dominate overall sales performance

✔ A small number of regions account for most order cancellations

These insights can help businesses improve:

Supply chain efficiency

Inventory planning

Regional sales strategies

🛠 Tools & Skills Demonstrated
Excel Analytics

Pivot Tables

Pivot Charts

Slicers

Calculated Fields

Excel Functions

XLOOKUP

IF

IFERROR

SUM

COUNT

AVERAGE

TEXT

Data Analysis Skills

Data Cleaning

Data Transformation

KPI Development

Dashboard Design

Business Insight Generation

📷 Dashboard Preview

(Add your dashboard screenshot here)

Example:

![Dashboard Preview](dashboard.png)
🚀 Why This Project Matters

This project demonstrates my ability to:

✔ Transform raw business data into meaningful insights
✔ Design interactive dashboards for decision-makers
✔ Apply analytical thinking to real business problems
✔ Use Excel as a powerful data analysis tool

👤 About Me

Aman Kumar

Aspiring Data Analyst | Business Analytics Enthusiast

I enjoy solving business problems using data analysis, visualization, and storytelling.

🔗 LinkedIn: (Add your link)
🔗 GitHub: (Add your GitHub profile)
