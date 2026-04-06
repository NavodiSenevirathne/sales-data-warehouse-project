# 📊 Sales Order Data Warehouse & BI Project

🚀 End-to-end **Data Warehousing & Business Intelligence solution** built using SQL Server, SSIS, SSAS, and Power BI.

---

## 🔍 Project Overview

This project demonstrates the complete pipeline of transforming raw transactional data into meaningful business insights.

It includes:
- Data Warehouse Design (Star Schema)
- ETL Pipeline Development (SSIS)
- OLAP Cube (SSAS)
- Dashboarding (Power BI & Excel)

The goal is to enable **data-driven decision-making** by converting OLTP data into an analytical model.

---

## 💼 Business Problem

Operational systems store data efficiently for transactions, but not for analytics.

👉 This project solves that by:
- Integrating data from multiple sources
- Transforming it into a structured data warehouse
- Enabling fast reporting and insights through dashboards

---

## 🗂 Dataset

This project uses the **WideWorldImporters** sample database provided by Microsoft.

🔗 Dataset Link:  
https://github.com/Microsoft/sql-server-samples/releases/tag/wide-world-importers-v1.0

- A real-world **OLTP database simulation**
- Contains data on customers, sales, products, and transactions
- Designed to demonstrate database design, ETL, and analytics workflows :contentReference[oaicite:0]{index=0}  

👉 It includes both:
- **WideWorldImporters (OLTP)** → transactional data  
- **WideWorldImportersDW (OLAP)** → analytics-ready data :contentReference[oaicite:1]{index=1}  

---

## 🏗 Solution Architecture

### 🔹 Components:
- **Source Systems:** SQL Server + CSV files  
- **Staging Area:** Temporary raw data storage  
- **Data Warehouse:** Star Schema model  
- **Reporting Layer:** SSAS Cube + Power BI dashboards  

---

## ⭐ Data Warehouse Design

### 📌 Schema: Star Schema

- **Fact Table:**  
  - `FactSales` (sales transactions)

- **Dimension Tables:**  
  - `DimCustomer`  
  - `DimProduct`  
  - `DimSalesperson`  
  - `DimDate`  

👉 Each record represents an **invoice line**, enabling detailed analysis.

---

## 🔄 ETL Process (SSIS)

ETL pipeline was built using **SQL Server Integration Services (SSIS)**.

### 🔹 Steps:
1. Extract data from:
   - SQL Server tables
   - CSV file
2. Load into staging tables
3. Transform:
   - Join datasets
   - Handle null values
   - Apply business rules
4. Load into fact & dimension tables

### ✔ Key Features:
- Data cleaning & validation  
- Lookup transformations  
- Referential integrity checks  

---

## 🔁 Slowly Changing Dimension (SCD Type 2)

Implemented for **Customer Dimension** to track historical changes.

✔ Tracks:
- Customer category changes  
- Location updates  
- Attribute history  

---

## 📊 SSAS Cube (OLAP)

Built a **Multidimensional Cube** using SSAS.

### 📌 Measures:
- Sales Amount  
- Profit  
- Quantity  
- Cost  
- Tax  

### 📌 Hierarchies:
- **Date:** Year → Quarter → Month → Day  
- **Location:** City → State → Country → Continent  

👉 Enables:
- Drill-down  
- Roll-up  
- Slice & Dice  
- Pivot analysis  

---

## 📈 Power BI Dashboard

Connected Power BI to the cube for interactive dashboards.

### 🔹 Insights:
- Sales trends over time  
- Customer segmentation  
- Product performance  
- Regional analysis  

📊 Enables real-time, interactive business analysis.

---

## 📊 Excel OLAP Analysis

Used PivotTables to demonstrate:
- Roll-up  
- Drill-down  
- Slice  
- Dice  
- Pivot  

---

## 🛠 Tech Stack

- SQL Server  
- SSIS (ETL)  
- SSAS (OLAP Cube)  
- Power BI  
- Excel  
- Data Warehousing  
- Star Schema  
- SCD Type 2  

---

## 🎯 Key Learnings

- Data warehouse design & dimensional modeling  
- ETL pipeline development  
- Data cleaning & validation  
- OLAP cube development  
- Dashboarding with Power BI  

---

## 👩‍💻 Author

**Navodi Senevirathne**  
Data Science Undergraduate | Aspiring Data Analyst  

---

## ⭐ If you like this project, feel free to star the repo!
