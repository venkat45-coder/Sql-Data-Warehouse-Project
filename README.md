# Data Warehouse and Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository! 🚀

This project demonstrates a comprehensive, end-to-end data warehousing and analytics solution — from raw data ingestion all the way through to business-ready reporting and insights. Built as a portfolio project, it showcases industry best practices across data engineering, data modeling, ETL pipeline development, and SQL-based analytics.

---

## 🏗️ Data Architecture

The project follows **Medallion Architecture**, organizing data across three progressive layers that take raw source data and refine it into analysis-ready business intelligence.

![Data Architecture]

- **Bronze Layer** — Raw data ingested as-is from source CSV files directly into a SQL Server database. No transformations are applied at this stage; the data is preserved exactly as received from source systems.
- **Silver Layer** — Data cleansing, standardization, and normalization are applied here. This layer resolves quality issues, removes duplicates, standardizes formats, and prepares data for reliable downstream use.
- **Gold Layer** — Business-ready data modeled into a **star schema** (fact and dimension tables), optimized for analytical queries, reporting, and dashboarding.

---

## 📖 Project Overview

This project covers the full lifecycle of a modern data warehousing solution across four core areas:

- **Data Architecture** — Designing a scalable Modern Data Warehouse using the Medallion Architecture (Bronze, Silver, Gold layers) to progressively refine raw data into analytical assets.
- **ETL Pipelines** — Extracting data from ERP and CRM source systems, applying transformation logic, and loading structured data into the warehouse across all three layers.
- **Data Modeling** — Developing fact and dimension tables in a star schema that are optimized for fast, flexible analytical queries across sales, customers, and products.
- **Analytics & Reporting** — Creating SQL-based reports and dashboards that surface actionable insights on customer behavior, product performance, and sales trends.

### 🎯 Skills Demonstrated

This repository is a strong portfolio reference for professionals and students looking to demonstrate expertise in:

- SQL Development
- Data Architecture
- Data Engineering
- ETL Pipeline Development
- Data Modeling
- Data Analytics

---

## 🛠️ Tools & Resources

All tools used in this project are **free to use**:

- **Datasets** — CSV files for ERP and CRM source data are included in the `/datasets` folder.
- **SQL Server Express** — Lightweight, free SQL Server instance used to host the data warehouse database.
- **SQL Server Management Studio (SSMS)** — GUI tool for writing queries, managing the database, and exploring schemas.
- **Git & GitHub** — Version control and collaboration platform used to manage all project code and documentation.
- **Draw.io** — Used to design and document data architecture diagrams, data flow diagrams, ETL flows, and data models.
- **Notion** — Project template and task tracker used to manage all project phases and milestones.

---

## 🚀 Project Requirements

### Part 1 — Building the Data Warehouse (Data Engineering)

**Objective:**
Develop a modern data warehouse using SQL Server to consolidate sales data from multiple source systems, enabling reliable analytical reporting and data-driven decision-making.

**Specifications:**

- **Data Sources** — Import and integrate data from two source systems (ERP and CRM), each provided as CSV files with distinct schemas and formats.
- **Data Quality** — Identify, cleanse, and resolve data quality issues — including missing values, duplicates, and format inconsistencies — before loading data into analytical layers.
- **Data Integration** — Combine both source systems into a single, unified data model that is intuitive, consistent, and designed for analytical queries.
- **Scope** — Focus on the latest snapshot of each dataset. Historical change tracking (SCD / historization) is out of scope for this project.
- **Documentation** — Deliver clear, comprehensive documentation of the data model, including a data catalog and naming conventions, to support both business stakeholders and analytics teams.

---

### Part 2 — Analytics & Reporting (Data Analysis)

**Objective:**
Develop SQL-based analytics to deliver detailed, actionable insights across three key business domains.

**Reporting Areas:**

- **Customer Behavior** — Analyze purchasing patterns, customer segmentation, loyalty trends, and lifetime value indicators.
- **Product Performance** — Measure revenue contribution, sales velocity, and performance trends across product categories and individual SKUs.
- **Sales Trends** — Identify seasonal patterns, period-over-period growth, and revenue distribution across time dimensions.

These insights provide business stakeholders with key metrics to support strategic planning and operational decision-making. For full details, refer to `docs/requirements.md`.

---

## 📂 Repository Structure

```
data-warehouse-project/
│
├── datasets/                        # Raw source datasets (ERP and CRM CSV files)
│
├── docs/                            # Project documentation and architecture assets
│   ├── etl.drawio                   # ETL techniques and methods diagram
│   ├── data_architecture.drawio     # Overall data architecture diagram
│   ├── data_catalog.md              # Dataset catalog with field descriptions and metadata
│   ├── data_flow.drawio             # End-to-end data flow diagram
│   ├── data_models.drawio           # Star schema and data model diagrams
│   └── naming-conventions.md        # Naming guidelines for tables, columns, and files
│
├── scripts/                         # SQL scripts for ETL and data transformation
│   ├── bronze/                      # Scripts for raw data extraction and loading
│   ├── silver/                      # Scripts for data cleansing and transformation
│   └── gold/                        # Scripts for creating analytical models
│
├── tests/                           # Data quality test scripts and validation files
│
├── README.md                        # Project overview and setup instructions
├── LICENSE                          # License information
├── .gitignore                       # Files and directories excluded from version control
└── requirements.txt                 # Project dependencies and requirements
```

---

## 🤝 Contributing

Contributions, suggestions, and feedback are welcome. Feel free to open an issue or submit a pull request if you'd like to improve any part of this project.

---

## 📄 License

This project is licensed under the terms specified in the `LICENSE` file.
