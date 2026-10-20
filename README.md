# ShopSmart Retail Ltd. | 2025 Sales Performance Analysis
### Interactive Excel Dashboard • Power Pivot • Data Modelling • DAX • Business Insights
#### Business Background

ShopSmart Retail Ltd. is a retail business operating across different locations in Nigeria, offering products in categories such as Beauty, Electronics, Fashion, Groceries, and Home. The company generates sales, customer, product, returns, and inventory data through its daily operations. Analysing this data can help management understand business performance and make better decisions.

### Problem Statement

ShopSmart needs a clearer understanding of its sales performance, customer spending patterns, product demand, returns, and inventory levels across its stores. Without a centralised view of these activities, management may struggle to identify top-performing products, underperforming stores, and potential stock shortages.

This project addresses these challenges by using **Excel and Power Pivot to analyse the company's 2025 data and build an interactive dashboard**

The project uses 50,000 orders, 5,000 customers, 500 products, and supporting store, supplier, returns and inventory tables. The dashboard includes slicers for Year, Month, Category, Membership Level and State.
# Dashboard

<img width="960" height="540" alt="Dashboard" src="https://github.com/user-attachments/assets/58a7813b-a3e5-4b27-8ce6-e15b9c99402b" />



# Tools and workflow
- **Microsoft Excel:** reviewed source tables, prepared analytical columns, created PivotTables, PivotCharts, KPI cards and slicers.
- **Power Pivot / Data Model:** connected the tables through their shared IDs and created reusable calculations.
- **DAX:** calculated revenue, order/customer metrics, returns and inventory value.
- **Dashboard design:** formatted financial figures in millions or billions and built an executive summary for business users.
I reviewed the data and column types, prepared revenue and inventory calculations, loaded the tables into the Data Model, established relationships, built PivotTables and measures, created the charts and KPI cards, connected slicers and interpreted the results.

# Power Pivot data model and Diagram View

<img width="960" height="540" alt="Data Modelling" src="https://github.com/user-attachments/assets/06575ab4-c603-40c3-a259-38870c2bf260" />

    Customers[ShopSmart_Customers] -->|Customer_ID · 1 to many| Orders[ShopSmart_Orders]
    Stores[ShopSmart_Stores] -->|Store_ID · 1 to many| Orders
    Orders -->|Order_ID · 1 to many| Items[ShopSmart_Order_Items]
    Products[ShopSmart_Products] -->|Product_ID · 1 to many| Items
    Orders -->|Order_ID · 1 to many| Returns[ShopSmart_Returns]
    Products -->|Product_ID · 1 to many| Inventory[ShopSmart_Inventory]
    Stores -->|Store_ID · 1 to many| Employees[ShopSmart_Employees]
    Stores -.->|Store_ID · inactive| Inventory

# Executive dashboard KPIs
### KPI	Full-year figure	Interpretation
- **Total Revenue**	₦7.58B	Sum of order-item line totals across recorded order statuses
- **Total Orders**	50K	Number of recorded orders
- **Total Customers**	5K	Customers represented in the dataset
- **Average Order Value**	₦151.51K	Average order value shown in the dashboard
- **Return Rate**	4.88%	Overall returns KPI
- **Inventory Value**	₦3.17B	Value of stock on hand at cost price

# Charts
# 1. Monthly Sales Trend — line chart
The line chart shows revenue from January through December and makes changes over time easy to see. December generated the highest monthly revenue, about ₦660.63M. This helps management plan promotions and stock availability around stronger periods.

<img width="245" height="109" alt="Monthly sales trend" src="https://github.com/user-attachments/assets/d74f3ec8-b7db-468b-afba-2b72490f6c89" />


# 2. Sales by State — horizontal bar chart
This chart compares revenue geographically. Lagos and Oyo are the highest performing state while kano is the lowest performing state It helps identify where demand is concentrated and where marketing or operational support may be useful.

<img width="185" height="111" alt="Sales by state" src="https://github.com/user-attachments/assets/5b49b68f-bea9-4716-9e25-88f1352b3030" />


# 3. Revenue by Store — horizontal bar chart
 ShopSmart Lagos led with approximately ₦1.23B, closely followed by Ibadan and Abuja. It supports store-performance comparisons and resource allocation.

<img width="227" height="134" alt="Revenue by store" src="https://github.com/user-attachments/assets/fb5eb4a9-6a86-4622-937d-e53632f0a317" />


# 4. Revenue by Category — column chart
The chart compares Beauty, Electronics, Fashion, Groceries and Home. Beauty ranked first at about ₦1.76B, followed by Groceries at about ₦1.58B. This highlights strong product categories, although profitability and return rates should also inform investment decisions.

<img width="191" height="131" alt="Revenue by catogory" src="https://github.com/user-attachments/assets/7dafb62b-de97-44f4-bb4b-f46feebe9e84" />

# 5. Revenue Top Products — horizontal bar chart
This chart ranks individual products by revenue. Home Item 400 generated approximately ₦21.64M, making it the top-revenue product in the full-year analysis. It helps identify products to monitor for availability and promotional opportunities.

<img width="183" height="240" alt="Revenue Top Product" src="https://github.com/user-attachments/assets/9c1fe630-73cc-4e81-905a-1d8c775d3198" />

# Business findings
## 1. Beauty was the leading revenue category, contributing approximately ₦1.76B.
## 2. ShopSmart Lagos was the strongest store, contributing approximately ₦1.23B, while the South region led overall regional performance at about ₦2.42B.
## 3. Inventory and returns need monitoring: some stock records were at or below their reorder levels, and some products were returned repeatedly.
# Recommendations
## 1. Support high-performing products and categories. Prioritise availability and targeted promotions for strong sellers, while checking margins before committing more investment.
## 2. Improve inventory planning. Monitor stock against reorder levels and prioritise replenishment where shortages are more likely.
## 3. Investigate returns and retain valuable customers. Review frequent-return products and use customer spending insights to design relevant loyalty offers.
## Risk: Stock shortages and recurring returns could reduce customer satisfaction and sales opportunities.

## Opportunity: Strong performance in Beauty and the South region offers a basis for targeted growth.
