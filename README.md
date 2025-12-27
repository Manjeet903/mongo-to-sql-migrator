# mongo-to-sql-migrator

# Mongo-to-SQL High-Performance Data Pipeline

A configuration-driven ETL tool designed to migrate large-scale transactional data from **MongoDB (NoSQL)** to **SQL Server** for analytical reporting.

## 🚀 Key Features
- **Dynamic Schema Validation:** Automatically detects source schema and creates SQL tables if they don't exist.
- **Batch Processing:** Utilizes `fast_executemany` for high-performance bulk insertions.
- **Config-Driven:** Mappings, pipelines, and database credentials are fully decoupled from the code.
- **Automated Logging:** Tracks success, failures, and batch metrics.
- **Failure Handling:** Includes transaction rollback mechanisms to ensure data integrity.

## 🛠 Tech Stack
- **Language:** Python 3.9+
- **Database:** MongoDB (Source), MS SQL Server (Target)
- **Libraries:** `pymongo`, `pyodbc`, `json`, `logging`

## ⚙️ How to Run
1. Clone the repo.
2. Install dependencies: `pip install pymongo pyodbc`
3. Rename `config.example.json` to `config.json` and update credentials.
4. Run the pipeline:
   ```bash
   python mongo_sql_etl.py
