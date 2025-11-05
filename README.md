# 🏢 Data Warehouse & Analytics Project

Welcome to the **Data Warehouse and Analytics Project**! 🚀  
A comprehensive end-to-end solution demonstrating modern data warehousing, ETL pipelines, and analytics using SQL Server. This portfolio project showcases industry best practices in data engineering and analytics, from raw data ingestion to actionable business insights.

---

## 🎯 Project Overview

This project delivers a complete data warehousing solution that consolidates sales data from multiple source systems, enabling analytical reporting and data-driven decision-making. Built with SQL Server, it demonstrates the full lifecycle of data engineering—from extraction to insight generation.

### What Makes This Project Special?

- 🏗️ **Modern Architecture**: Implements Medallion Architecture with Bronze, Silver, and Gold layers
- 🔄 **Complete ETL Pipeline**: End-to-end data transformation workflows
- ⭐ **Star Schema Design**: Optimized dimensional modeling for analytics
- 📊 **Business Intelligence**: SQL-based analytics delivering actionable insights
- 📚 **Portfolio-Ready**: Comprehensive documentation and best practices
- 🆓 **100% Free**: All tools and resources are completely free to use

---

## 🏗️ Architecture
This project follows the **Medallion Architecture** pattern, organizing data into three distinct layers:
---
<img width="1006" height="621" alt="DWH Project drawio" src="https://github.com/user-attachments/assets/77dbec8b-f102-43a6-b149-002116674e4a" />


### 📦 Bronze Layer (Raw Data)
Stores data exactly as received from source systems with no transformations. This layer ensures data lineage and enables reprocessing if needed.
- **Source**: CSV files from ERP and CRM systems
- **Destination**: SQL Server Database tables
- **Purpose**: Data preservation and historical record

### 🔧 Silver Layer (Refined Data)
Applies data quality processes including cleansing, standardization, and normalization to prepare data for analysis.
- **Processes**: Data validation, deduplication, type conversion
- **Quality Rules**: Enforced business rules and data constraints
- **Purpose**: Clean, consistent data ready for modeling

### 🌟 Gold Layer (Business-Ready Data)
Contains analytically-optimized data modeled into star schema with fact and dimension tables.
- **Model**: Star schema design for optimal query performance
- **Content**: Business-ready aggregations and metrics
- **Purpose**: Enable reporting, dashboards, and analytics

---

## ✨ Features

### Data Engineering Capabilities
- 🔄 **ETL Pipelines**: Automated extraction, transformation, and loading processes
- 🎯 **Data Quality**: Built-in validation and cleansing workflows
- 🏗️ **Data Modeling**: Star schema with optimized fact and dimension tables
- 📈 **Scalability**: Designed to handle growing data volumes

### Analytics & Insights
- 👥 **Customer Behavior Analysis**: Deep dive into customer patterns and trends
- 📦 **Product Performance**: Track and analyze product sales metrics
- 📊 **Sales Trends**: Identify seasonal patterns and growth opportunities
- 💡 **Business Metrics**: KPIs and measures for strategic decision-making

### Professional Development
Perfect for showcasing expertise in:
- SQL Development & Query Optimization
- Data Architecture & Design
- ETL Pipeline Development
- Dimensional Modeling
- Data Analytics & Reporting

---

## 🚀 Quick Start

Get the project running in minutes:

```sql
-- 1. Create the database
CREATE DATABASE DataWarehouse;
GO

-- 2. Run Bronze layer scripts (raw data ingestion)
-- Execute scripts in: scripts/bronze/

-- 3. Run Silver layer scripts (data transformation)
-- Execute scripts in: scripts/silver/

-- 4. Run Gold layer scripts (analytical models)
-- Execute scripts in: scripts/gold/

-- 5. Start analyzing!
-- Use queries from analytics scripts
```

---

## 📦 Requirements

### Building the Data Warehouse (Data Engineering)

**Objective**: Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical reporting and informed decision-making.

**Specifications**:
- **Data Sources**: Import data from two source systems (ERP and CRM) provided as CSV files
- **Data Quality**: Cleanse and resolve data quality issues prior to analysis
- **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries
- **Scope**: Focus on the latest dataset only; historization of data is not required
- **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics teams

### BI: Analytics & Reporting (Data Analysis)

**Objective**: Develop SQL-based analytics to deliver detailed insights into:

- 👥 **Customer Behavior**: Purchase patterns, segmentation, and lifetime value
- 📦 **Product Performance**: Best sellers, inventory turnover, and profitability
- 📈 **Sales Trends**: Time-series analysis, forecasting, and growth metrics

These insights empower stakeholders with key business metrics, enabling strategic decision-making.

📖 For complete requirements, see [docs/requirements.md](docs/requirements.md)

---

## 🛠️ Installation

### Prerequisites

Ensure you have the following tools installed (all free!):

1. **[SQL Server Express](https://www.microsoft.com/sql-server/sql-server-downloads)** - Lightweight database server
2. **[SQL Server Management Studio (SSMS)](https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms)** - Database management GUI
3. **[Git](https://git-scm.com/)** - Version control system
4. **[Draw.io](https://www.drawio.com/)** - For viewing architecture diagrams (optional)

### Step-by-Step Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/DataWithBaraa/data-warehouse-project.git
   cd data-warehouse-project
   ```

2. **Set Up SQL Server**
   - Install SQL Server Express
   - Install SQL Server Management Studio (SSMS)
   - Connect to your local SQL Server instance

3. **Create the Database**
   ```sql
   CREATE DATABASE DataWarehouse;
   GO
   USE DataWarehouse;
   GO
   ```

4. **Execute Scripts in Order**
   - **Bronze Layer**: Run scripts from `scripts/bronze/` to load raw data
   - **Silver Layer**: Run scripts from `scripts/silver/` to clean and transform
   - **Gold Layer**: Run scripts from `scripts/gold/` to create analytical models

5. **Verify Installation**
   - Check that all tables are created
   - Run test queries from `tests/` directory

---


</div>
