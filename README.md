# AzureProject
# 🏎️ Formula 1 Data Engineering Project using Databricks & Azure Data Factory

This project demonstrates a complete end-to-end **data pipeline solution** using **Azure Data Lake Storage (ADLS)**, **Databricks**, and **Azure Data Factory (ADF)**. The goal is to simulate a real-world Formula 1 analytics workflow that ingests, transforms, and moves data across cloud services.

---

## 🚀 Project Overview

### 👨‍💻 What I Did
- Ingested raw **Formula 1 racing data** from **Azure Data Lake** into **Databricks**
- Used **PySpark** in Databricks to filter and transform data
- Connected storage using multiple methods:
  - 🔑 Access Key
  - 🔐 Shared Access Signature (SAS)
  - 🛡️ Azure Access Token
- Managed secrets using **Azure Key Vault**
- Built **ADF pipelines** to automate and schedule data movement
- Enabled **GitHub integration** in ADF for version control and collaboration

---

## 🛠️ Tools & Technologies

| Tool                        | Purpose                                      |
|----------------------------|----------------------------------------------|
| **Azure Data Lake Storage (ADLS)** | Cloud-based data storage             |
| **Azure Databricks**       | Data transformation and PySpark processing   |
| **Azure Data Factory (ADF)** | Pipeline orchestration and automation      |
| **Azure Key Vault**        | Credential management                        |
| **Power BI**               | Data visualization and reporting             |
| **GitHub**                 | Version control and project tracking         |


---

## 📂 Project Structure (in Databricks)

| 📂 Folder    | 📄 Contents / Purpose                                                               |
| ------------ | ----------------------------------------------------------------------------------- |
| `analysis/`  | Contains data analysis and visualization notebooks               |
| `demo/`      | Contains SQL and Delta Lake demo notebooks (e.g., `filter_demo`, `join_demo`, etc.) |
| `includes/`  | Utility notebooks like `common_functions` and `configuration`                       |
| `ingestion/` | Data ingestion logic (used to bring raw from ADLS into Databricks) |
| `raw/`       |Contains notebook to create Tables like f1_raw.drivers from JSON files using schema-on-read (e.g., create_raw_tables) |
| `set-up/`    | Setup notebooks for configuring ADLS access (access keys, SAS, service principal)   |
| `trans/`     | Transformation logic like `race_results`, `driver_standings`, `calc_race_results`   |
| `utils/`     | Likely contains helper functions or reusable code modules                           |

