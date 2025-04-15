
# 🧾 Data Warehouse Naming Conventions Guide

A standardized naming convention ensures consistency, clarity, and maintainability across all objects in your data warehouse. This document outlines the rules followed in the **Data Warehouse & Analytics Project** led by **Nitin Rawat**.

---

## 📚 Table of Contents

- [🧠 General Principles](#-general-principles)  
- [📦 Table Naming Conventions](#-table-naming-conventions)  
  - [🟫 Bronze Layer](#-bronze-layer)  
  - [⬜ Silver Layer](#-silver-layer)  
  - [🥇 Gold Layer](#-gold-layer)  
- [📌 Column Naming Conventions](#-column-naming-conventions)  
  - [🧱 Surrogate Keys](#-surrogate-keys)  
  - [⚙️ Technical Columns](#-technical-columns)  
- [🛠️ Stored Procedure Naming](#️-stored-procedure-naming)  
- [🧾 Glossary of Prefixes](#-glossary-of-prefixes)

---

## 🧠 General Principles

- ✅ **Use `snake_case`**: All object names must be in lowercase and use underscores to separate words.  
- ✅ **Use English**: Maintain English language for universal understanding.  
- 🚫 **Avoid SQL Reserved Words**: Never use reserved keywords as object names.

---

## 📦 Table Naming Conventions

### 🟫 Bronze Layer

- **Pattern**: `<source_system>_<entity>`  
- **Rule**: Use the exact original table name from the source system. Do not rename.  
- **Example**:  
  `crm_customer_info` → Raw CRM customer data  
  `erp_sales_orders` → Raw ERP order data

---

### ⬜ Silver Layer

- **Pattern**: `<source_system>_<entity>`  
- **Rule**: Retain source naming. This layer involves cleansed and standardized data but keeps the original structure.  
- **Example**:  
  `erp_products_master` → Cleaned ERP product data  
  `crm_customer_info` → Cleaned CRM customer records

---

### 🥇 Gold Layer

- **Pattern**: `<category>_<entity>`  
- **Rule**: Use business-friendly, analytics-ready names aligned with dimensional modeling.

#### Examples:
- `dim_customers` → Dimension table for customer data  
- `dim_products` → Dimension table for products  
- `fact_sales` → Fact table for sales transactions  
- `report_sales_monthly` → Aggregated reporting table

---

## 📌 Column Naming Conventions

### 🧱 Surrogate Keys

- **Pattern**: `<table_name>_key`  
- **Use**: Unique, system-generated primary keys for dimension tables.  
- **Example**:  
  `customer_key` → Primary key in `dim_customers`  
  `product_key` → Primary key in `dim_products`

---

### ⚙️ Technical Columns

- **Pattern**: `dwh_<column_name>`  
- **Use**: Metadata for data lineage and tracking.  
- **Example**:  
  `dwh_load_date` → Load timestamp  
  `dwh_source_file` → Origin filename

---

## 🛠️ Stored Procedure Naming

- **Pattern**: `load_<layer>`  
- **Use**: Script names used for loading data into each layer of the warehouse.  

#### Examples:
- `load_bronze` → Handles raw data ingestion  
- `load_silver` → Handles data cleansing and transformation  
- `load_gold` → Handles dimensional modeling and aggregation


## 📬 Maintainer

Maintained by **Nitin Rawat** — Data Analyst | Data Engineer  
📍 Delhi, India  
🔗 [LinkedIn](https://www.linkedin.com/in/nitin-rawat-a38536270/) | [GitHub](https://github.com/nitinrawat05) | ✉️ nitinrawat2502@gmail.com

---

> 🧠 *Consistent naming is not just style — it’s a practice that enables better communication, faster onboarding, and fewer mistakes in data-driven environments.*

