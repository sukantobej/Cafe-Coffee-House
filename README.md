# ☕ Cafe Coffee House - Sales Dashboard Project

This project presents a comprehensive dashboard for **Cafe Coffee House**, designed to analyze and visualize business performance using key sales and customer insights. It provides a snapshot of operational metrics, helping stakeholders make informed decisions based on real-time data.

📌**Project Overview**

Cafe Coffee House is a premium café chain offering a wide range of beverages and snacks. The goal of this project is to build a comprehensive, interactive Excel dashboard to help stakeholders analyze key performance metrics like total sales, footfall, average billing, product performance, and category trends. This data-driven dashboard aids in making informed business decisions, optimizing peak operating hours, product offerings, and promotional strategies.

🚀 **Process of Creating the Dashboard**

1️⃣ **Data Extraction & Cleaning**

Collected raw sales, product, and store location data.

Removed whitespace, duplicates, and standardized column formats.

Validated and corrected data types (e.g., dates, numerical fields).

Ensured consistency and completeness for critical dimensions like product categories and timestamps.

2️⃣ **Data Transformation & Feature Engineering**

Extracted new dimensions such as:

Month and Day Name from Order Date for seasonal trend analysis.

Hour of Order to identify high-traffic business hours.

Hour of Delivery to determine preferred delivery slots.

Calculated:

Delivery Time Lag = Delivery Date - Order Date (in days).

Revenue = Quantity × Price.

3️⃣ **Data Modeling**

Merged multiple tables using primary keys such as Product ID and Customer ID.

Applied Star Schema modeling:

Fact Table: Orders (with metrics like quantity, revenue).

Dimension Tables: Customers, Products, Time.

Implemented DAX/Excel formulas for calculated fields and formatted time dimensions using:

excel
Copy
Edit
=FORMAT(Order[Order_Date],"DDDD")
4️⃣ **Pivot Tables & Insights Generation**

Created key pivot tables to drive dashboard metrics:

Total Revenue and Quantity Ordered.

Footfall and Revenue by Store Location.

Sales by Product Size (Small, Regular, Large, Not Defined).

Category-wise Revenue Contribution.

Top 5 Products by Sales.

Orders and Revenue by Weekdays.

5️⃣ **Visualization & Dashboard Design**

Built an interactive Excel dashboard with user-friendly slicers:

Filters for Month, Day, and Product Category.

Applied custom color palettes and card-style visuals for KPIs:

Total Sales, Footfall, Avg Orders/Person, Avg Bill/Person.

Locked and protected sheets to prevent accidental edits.

Utilized combo charts, pie charts, and bar graphs for rich visual storytelling.

📊 **Key Business Insights**
Total Sales: $6,98,812.33 with a total footfall of 149,116.

Avg Order/Person: 1.44 | Avg Bill/Person: $4.69

Peak Order Hours: Between 8 AM - 11 AM, with quantities over 25k.

Popular Products: Barista Espresso, Brewed Chai Tea, and Hot Chocolate lead the sales.

Category Performance:

Coffee dominates with 38.63% share.

Tea and Branded products also contribute significantly.

Sales by Size: Regular (30.71%) and Large (30.10%) are the most preferred drink sizes.

Weekday Revenue: Steady throughout the week with slight peaks on Friday and Monday.

Top Store Locations: Hell’s Kitchen and Astoria perform best in both footfall and revenue.

🛠️ **Tools Used**  
- Excel (Power Query, Data Modeling, Pivot Tables)  
- Data Cleaning & Transformation    
- Data Visualization & Dashboarding

  
📎 **Conclusion**
This project demonstrates how Excel can be used as a powerful business intelligence tool. By consolidating sales data into a visually rich and interactive dashboard, Cafe Coffee House can drive better business decisions, identify sales trends, optimize operations, and improve customer experience.
  
