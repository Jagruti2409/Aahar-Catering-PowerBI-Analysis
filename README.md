
Aahar Catering – Power BI Business Analytics Dashboard
📌 Project Overview

This project presents a 1-year business performance analysis for Aahar Catering, operating across Chh. Sambhajinagar, Saputara, Dhule and nearby regions.
The dashboard provides data-driven insights into revenue, event performance, and customer trends using Power BI.

The objective is to help catering businesses make better decisions using visual analytics.

🛠️ Tools & Technologies Used

Power BI

Power Query

DAX (Data Analysis Expressions)

Excel / CSV (Data Source)

Data Modelling (Star Schema)

📊 Key Insights

✔ Event Type comparison (Wedding, Engagement, Corporate, Other)

✔ Total Revenue & Yearly Growth

✔ Monthly Sales Trend Analysis

✔ Location-wise Performance

✔ Top Clients & High-Value Events

✔ Interactive Filters for dates, event types, and regions


🗂️ Project Structure

Aahar Catering - Sample Dataset Pack
Generated for: Aahar Catering (Chh. Sambhajinagar area)
Period: 2024-01-01 to 2024-12-31
Currency: INR

Files included (saved in this folder):
- Sales_Data.xlsx : Orders with revenue, estimated cost and profit per order.
- Menu_Items.xlsx : Menu items with cost and selling price.
- Customer_Data.xlsx : Customer master list.
- Expenses_Data.xlsx : Monthly + event-specific expenses.
- Staff_Data.xlsx : Staff master data.
- Data_Dictionary.xlsx : Column explanations and data mapping.

Power BI tips:
1. Import all Excel tables into Power BI and mark Date columns as Date type.
2. Create relationships:
   - Sales_Data[Customer_ID] -> Customer_Data[Customer_ID]
   - Sales_Data[Package_Name] -> (Packages are in Sales data; use Package_Name directly)
3. Measures to create in Power BI (DAX):
   - Total Sales = SUM(Sales_Data[Total_Sales_INR])
   - Total Cost = SUM(Sales_Data[Estimated_Cost_INR]) + SUM(Expenses_Data[Amount])
   - Gross Profit = SUM(Sales_Data[Gross_Profit_INR])
   - Net Profit = [Total Sales] - SUM(Expenses_Data[Amount])
   - Average Order Value = DIVIDE([Total Sales], DISTINCTCOUNT(Sales_Data[Order_ID]))
4. Use City and Event_Type slicers for drill-down analysis.


📸 Dashboard Preview

(Add images in the Screenshots folder)

📥 How to Use This Project

Download the .pbix file

Open it in Microsoft Power BI Desktop

If required, update data sources

Explore the interactive dashboard

🚀 What I Learned

Building professional business dashboards

Creating KPIs using DAX

Designing clean and interactive visuals

Data cleaning and transformation in Power Query

Understanding business metrics for catering/event industry
