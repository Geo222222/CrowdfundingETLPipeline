# 🧪 Crowdfunding ETL Pipeline

## 📦 Overview

This project involves building an **ETL (Extract, Transform, Load)** pipeline for crowdfunding campaign data. The objective is to extract raw campaign and category/subcategory data from CSV files, transform them into a clean format, and load them into a PostgreSQL relational database for structured querying.

---

## 🧰 Technologies

- Python
- Pandas
- PostgreSQL
- SQLAlchemy
- Jupyter Notebook

---

## 📁 Project Structure

```
crowdfunding_etl/
├── crowdfunding_db_schema.sql     # SQL schema with table definitions
├── crowdfunding_ETL.ipynb         # ETL pipeline script in notebook form
├── Resources/
│   ├── crowdfunding.csv           # Raw crowdfunding data
│   └── category.csv               # Category/subcategory mapping
├── README.md                      # Project documentation
```

---

## ⚙️ ETL Process

### 🔹 Extract
- Loaded CSV data for campaigns and category mappings
- Verified structure and contents of both datasets

### 🔹 Transform
- Parsed category and subcategory columns into a separate mapping
- Converted goal amounts and timestamps to standard formats
- Cleaned null values and filtered irrelevant records

### 🔹 Load
- Defined schema with table relationships
- Used SQLAlchemy to connect and push data into PostgreSQL
- Verified data integrity via SQL joins and SELECT statements

---

## 🗃️ Database Schema

Tables:
- `contacts`
- `campaign`
- `category`
- `subcategory`

Relationships are defined using primary and foreign keys for normalized structure.

---

## 🚀 How to Run

1. Clone the repo:
```bash
git clone https://github.com/Geo222222/Crowdfunding_ETL.git
cd Crowdfunding_ETL
```

2. Set up a PostgreSQL database locally (name: `crowdfunding_db`)

3. Execute `crowdfunding_db_schema.sql` to build tables

4. Run the ETL pipeline notebook to load data

---

## 📌 Enhancements

- Automate ETL process using a Python script or Airflow DAG
- Add data validation and logging
- Create a dashboard to monitor campaign performance

---

**Author:** [Geo222222](https://github.com/Geo222222)  
**Focus:** Data Engineering • ETL Pipelines • Relational Databases

