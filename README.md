
# 📊 Retail Sales & Profitability Analysis

## 📖 Project Overview

This project focuses on analyzing retail sales data to uncover actionable insights regarding sales performance, profitability, customer behavior, and regional trends. The dashboard provides a comprehensive view of business health, allowing stakeholders to monitor key performance indicators (KPIs), track profit margins, and identify top-performing products and regions.

## 🗂️ Data Architecture & Modelling

The dataset was already clean and required no major duplicate-removal or cleaning operations. The analysis is built upon a robust Star Schema dimensional model in Power BI to ensure efficient aggregations and clear relationships.

## [⭐ Star Schema Design](https://github.com/user-attachments/assets/f38157d9-5c66-4c48-913d-7743cacbc48e)

The data is organized into a central fact table surrounded by descriptive dimension tables:

### Central Fact Table:

* fact_sales: OrderID, CustomerID, ProductID, OrderDate, PaymentMethod, Quantity, Discount%, Profit, CustomerRating, Sales.

### Dimension Tables:

* dim_customer: CustomerID, CustomerName, CustomerSegment, Gender, AgeGroup, MembershipYears, Region.

* dim_product: ProductID, Product, Brand, Category, Supplier, UnitPrice.

* Dim_calendar_date: Date, Month Number, Month-Year.

## 📈 Dashboard Features 

### [Executive Summary](https://github.com/user-attachments/assets/ffb57549-1df9-402c-ba2b-cca48bf2d9e4)


* KPIs: Total Sales (3M), Total Profit (548K), Profit Margin (0.22), Total Orders (100), Average Customer Rating (4.46).

* Sales & Profit Trend Over Time: Line chart tracking performance across Jan 2025 to Apr 2025.

* Profit Distribution by Category: Donut chart highlighting Electronics (73.58%), Furniture (21.14%), Grocery (3.15%), and Clothing (2.1%).

* Total Sales by Region: Bar chart showing North (774K), West (681K), South (561K), and East (489K).

* Sales by Product & Category: Treemap visualization breaking down products (P001, P002, P005, etc.) within their respective categories.

* Average Customer Rating by Age Group: Bar chart comparing ratings across 18-25 (4.07), 25-35 (4.53), and 35-45 (4.80).

* Interactive Slicers: Region filters (East, North, South, West) and a "Clear all slicers" button.

### [Detailed Analysis](https://github.com/user-attachments/assets/1d924233-068f-42de-8633-a9dbe97000ef)


* Profit by Product: Bar chart ranking products by profit (P001 leading at 194K).

* Sales by Product: Bar chart showcasing sales volume per product (Laptop: 836K, TV: 502K, Mobile: 451K, Sofa: 238K, Chair: 170K).

* Brand-wise Profit by Month: Matrix table detailing brand performance (Ashirvad, Dell, Fortune, HomeCentre, IKEA, Levi's, LG, Pepehrry, Samsung) and Total Profit.

* Orders by Payment Method: Donut chart split by Credit Card (50%), UPI (21%), Cash (16%), and Debit Card (13%).

* Profit Margin & Sales Count by Brand: Combo chart (Line & Clustered Column) analyzing brand efficiency (Dell, LG, Samsung, Pepehrry, IKEA, HomeCentre, Levi's, Ashirvad, Fortune).

* Sales by Gender & Region: Stacked bar chart illustrating purchasing habits across Male and Female demographics.

* Interactive Slicers: Brand and Product dropdown filters.

### Data Matrix & Detail View

* KPIs: Total Sales, Total Profit, Profit Margin %.

* Detailed Table: A comprehensive matrix view showing Brand, Category, Product, Supplier, Region, Total Sales, Total Profit, and Profit Margin %.

* Slicers: Deep-dive filters for Brand, Category, Product, Supplier, and Region.

* Summary Totals (Filtered): Total Sales (774,470), Total Profit (172,300), Profit Margin (0.22).


## 🛠️ Tools & Technologies

Power BI Desktop: For data visualization, DAX calculations, and dashboard design.

Data Modeling: Star Schema implementation.

Data Source: Cleaned Retail Sales Dataset (Excel/CSV/SQL).



## 💡 Key Business Insights

* Electronics is the most profitable category, contributing over 73% of total profit.

* North Region generates the highest sales (774K), while the West follows closely (681K).

* Laptops are the highest-selling product (836K), significantly outperforming TVs and Mobiles.

* Credit Cards are the most preferred payment method (50% of orders).

* Customer ratings improve with age, with the 35-45 age group giving the highest average rating (4.80).

## 🚀 How to Use

Clone this repository.

Open the .pbix file in Power BI Desktop.

Ensure the data source paths are updated to your local directory if required.

Use the slicers on the left/right panels to filter the data dynamically across all three report pages.



