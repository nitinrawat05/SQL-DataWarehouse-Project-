# Data Warehouse and Analytics Project 🚀

Welcome to the **Data Warehouse and Analytics Project** repository! This project demonstrates a comprehensive data warehousing and analytics solution, from building a data warehouse to generating actionable insights. It is designed as a portfolio project, highlighting industry best practices in **data engineering** and **analytics**.

---

## 🏗️ Data Architecture

The project follows the **Medallion Architecture** with three key layers to process and transform the data:

### **Bronze Layer**: Raw Data Ingestion
- Stores data as-is from the source systems without any transformation.
- Data is ingested from **CSV files** and loaded into a **SQL Server Database** for further processing.

### **Silver Layer**: Data Cleansing and Transformation
- Data is cleaned, standardized, and normalized.
- This layer prepares the data for deeper analysis by ensuring consistency and usability.

### **Gold Layer**: Business-Ready Data
- Transformed data is modeled into a **star schema**, optimized for reporting and analytics.
- It contains data that is ready for use in generating actionable insights and supporting business decisions.

# 📖 Project Overview

This project involves:

- **Data Architecture**: Designing a Modern Data Warehouse Using Medallion Architecture (Bronze, Silver, and Gold layers).
- **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse.
- **Data Modeling**: Developing fact and dimension tables optimized for analytical queries.
- **Analytics & Reporting**: Creating SQL-based reports and dashboards for actionable insights.

🎯 This repository is an excellent resource for professionals and students looking to showcase expertise in:

- SQL Development
- Data Architecture
- Data Engineering
- ETL Pipeline Development
- Data Modeling
- Data Analytics



# Project Requirements

## Building the Data Warehouse 

### Objective
Develop a modern data warehouse using **SQL Server** to consolidate sales data, enabling analytical reporting and informed decision-making.

### Specifications
- **Data Sources**: Import data from two source systems (**ERP** and **CRM**) provided as **CSV files**.
- **Data Quality**: Cleanse and resolve data quality issues prior to analysis.
- **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries.
- **Scope**: Focus on the latest dataset only; historization of data is not required.
- **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics teams.


# BI: Analytics & Reporting (Data Analysis)

### Objective
Develop SQL-based analytics to deliver detailed insights into:

- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

These insights empower stakeholders with key business metrics, enabling strategic decision-making.

## 🗂️ Repository Structure

```bash
data-warehouse-project/
│
├── dataset/
│   ├── crm_csv/                         # CRM data in CSV format
│   │   ├── cust_info.csv
│   │   ├── prd_info.csv
│   │   ├── sales_details.csv
│   │   └── placeholder
│   └── erp_csv/                         # ERP data in CSV format
│       ├── CUST_AZ12.csv
│       ├── LOC_A101.csv
│       ├── PX_CAT_G1V2.csv
│       └── placeholder
│
├── docs/                                # Documentation and architecture diagrams
│   ├── architectureer.drawio
│   ├── data_flow.drawio
│   ├── integration_model.drawio
│   ├── holder
│   └── readme.md
│
├── script/                              # SQL scripts categorized by layer
│   ├── bronze/                          # Raw data ingestion scripts
│   │   ├── ddl_bronze_script.sql
│   │   └── proc_load_bronze.sql
│   ├── silver/                          # Data cleaning and transformation scripts
│   │   ├── create-silver-tables.sql
│   │   └── placeholder
│   └── gold/                            # Business-ready data modeling (star schema)
│       ├── gold.dim_products.sql
│       ├── gold_dim.sql
│       └── gold_layer_fact_sales_view.sql
│
├── test/                                # Test scripts and quality checks
│
├── LICENSE                              # MIT License
└── README.md                            # Project overview and instructions


# 🌟 About Me

Hi there! I'm **Nitin Rawat**, an experienced **Data Analyst** with a passion for turning data into actionable insights. I specialize in **SQL**, **Python**, and **Data Visualization** using **Tableau** and **Power BI**. I enjoy solving complex problems and making data-driven decisions to drive business growth.

Let's stay in touch! Feel free to connect with me on the following platforms:

