 Data Warehouse and Analytics Project 🚀

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
