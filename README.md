# 📊 Adventure Works Sales Analytics Dashboard

<p align="center">
  <img src="AdventureWork Dashboard.png" alt="Adventure Works Dashboard" width="100%">
</p>

## 📌 Project Overview

The Adventure Works Sales Analytics Dashboard is an end-to-end Data Analytics project developed using **MySQL** and **Power BI**. This project analyzes sales transactions, customer demographics, product performance, and return trends to generate actionable business insights.

The dashboard helps stakeholders track revenue, profit, customer behavior, product performance, and regional sales trends through interactive visualizations.

---

## 🎯 Objectives

* Analyze overall sales performance.
* Identify top-performing products and categories.
* Understand customer demographics and purchasing behavior.
* Evaluate regional sales performance.
* Monitor product returns and return rates.
* Build an interactive business intelligence dashboard.

---

## 🛠️ Tools & Technologies

| Tool             | Purpose                       |
| ---------------- | ----------------------------- |
| MySQL Workbench  | Database Management           |
| SQL              | Data Cleaning & Data Modeling |
| Power BI Desktop | Dashboard Development         |
| Microsoft Excel  | Data Validation               |

---

## 📂 Dataset

The project uses the Adventure Works dataset consisting of:

| Dataset                   | Description            |
| ------------------------- | ---------------------- |
| Adventure Works.csv       | Sales Transactions     |
| Customers.csv             | Customer Information   |
| Products.csv              | Product Details        |
| Product_Categories.csv    | Product Categories     |
| Product_Subcategories.csv | Product Subcategories  |
| Territories.csv           | Sales Territories      |
| Returns.csv               | Product Return Records |
| Calendar.csv              | Date Dimension         |

---

## 🗄️ Database Design

### Fact Tables

* Sales
* Returns

### Dimension Tables

* Customers
* Products
* Product Categories
* Product Subcategories
* Territories
* Calendar

### Database Operations Performed

* Imported CSV files into MySQL Workbench
* Created Primary Keys
* Established Foreign Key Relationships
* Built Star Schema Model
* Connected MySQL Database with Power BI

---

## 🔑 SQL Commands Used

### Create Database

```sql
CREATE DATABASE AdventureWorks;
USE AdventureWorks;
```

### Primary Keys

```sql
ALTER TABLE product_categories
ADD PRIMARY KEY (ProductCategoryKey);

ALTER TABLE product_subcategories
ADD PRIMARY KEY (ProductSubcategoryKey);

ALTER TABLE products
ADD PRIMARY KEY (ProductKey);

ALTER TABLE customers
ADD PRIMARY KEY (CustomerKey);

ALTER TABLE territories
ADD PRIMARY KEY (SalesTerritoryKey);

ALTER TABLE calendar
ADD PRIMARY KEY (Date);
```

### Foreign Keys

```sql
ALTER TABLE product_subcategories
ADD CONSTRAINT fk_subcat_category
FOREIGN KEY (ProductCategoryKey)
REFERENCES product_categories(ProductCategoryKey);

ALTER TABLE products
ADD CONSTRAINT fk_product_subcategory
FOREIGN KEY (ProductSubcategoryKey)
REFERENCES product_subcategories(ProductSubcategoryKey);

ALTER TABLE sales
ADD CONSTRAINT fk_sales_product
FOREIGN KEY (ProductKey)
REFERENCES products(ProductKey);

ALTER TABLE sales
ADD CONSTRAINT fk_sales_customer
FOREIGN KEY (CustomerKey)
REFERENCES customers(CustomerKey);

ALTER TABLE sales
ADD CONSTRAINT fk_sales_territory
FOREIGN KEY (TerritoryKey)
REFERENCES territories(SalesTerritoryKey);

ALTER TABLE returns_data
ADD CONSTRAINT fk_returns_product
FOREIGN KEY (ProductKey)
REFERENCES products(ProductKey);

ALTER TABLE returns_data
ADD CONSTRAINT fk_returns_territory
FOREIGN KEY (TerritoryKey)
REFERENCES territories(SalesTerritoryKey);
```

---

## 📈 Dashboard KPIs

| KPI               | Value  |
| ----------------- | ------ |
| Revenue           | 23.64M |
| Profit            | 9.73M  |
| Orders            | 14K    |
| Customers         | 9K     |
| Returned Products | 429    |
| Return Rate       | 3.08%  |
| Products          | 97     |

---

## 📊 Dashboard Features

### Revenue Analysis

* Revenue by Year
* Revenue by Category
* Revenue by Country

### Product Analysis

* Top 10 Products by Revenue
* Product Category Performance

### Customer Analysis

* Revenue by Gender
* Revenue by Occupation
* Customer Segmentation

### Return Analysis

* Return Quantity
* Return Rate Percentage

### Interactive Filters

* Date Range
* Year
* Category
* Gender
* Occupation

---

## 🔍 Key Business Insights

### Revenue Performance

* Total Revenue reached **23.64M**.
* Revenue peaked during **2016**.
* Strong sales growth was observed across multiple product categories.

### Product Performance

* **Bikes** generated the highest revenue.
* Mountain-200 series products were among the top-selling products.

### Customer Insights

* Revenue contribution from male and female customers was nearly balanced.
* Professional customers generated the highest revenue.

### Regional Performance

* United States generated the highest revenue.
* Australia ranked second in overall sales contribution.

### Returns Analysis

* Return Rate remained low at **3.08%**, indicating strong customer satisfaction and product quality.

---

## 📷 Dashboard Preview

### Executive Sales Dashboard

<p align="center">
  <img src="AdventureWork Dashboard.png" alt="Adventure Works Dashboard" width="100%">
</p>

---

## 🚀 Project Workflow

### Step 1: Data Collection

Collected Adventure Works CSV datasets.

### Step 2: Data Import

Imported datasets into MySQL Workbench.

### Step 3: Data Modeling

Created relationships using Primary Keys and Foreign Keys.

### Step 4: Power BI Integration

Connected MySQL database to Power BI Desktop.

### Step 5: Dashboard Development

Created KPIs, charts, slicers, and interactive visualizations.

### Step 6: Business Insights

Generated insights to support decision-making.

---

## 📁 Repository Structure

```text
AdventureWork-Analytics/
│
├── README.md
├── AdventureWork.pbix
├── AdventureWork Dashboard.png
│
└── Dataset/
    ├── Adventure Works.csv
    ├── Customers.csv
    ├── Products.csv
    ├── Product_Categories.csv
    ├── Product_Subcategories.csv
    ├── Territories.csv
    ├── Returns.csv
    └── Calendar.csv
```

---

## 👨‍💻 Author

**Anjith Kumar Bathala**

B.Tech – Computer Science Engineering (AI & ML)

### Skills

* SQL
* MySQL
* Power BI
* Data Analytics
* Machine Learning
* Artificial Intelligence

### GitHub

https://github.com/anjithkumar-3ab

---
