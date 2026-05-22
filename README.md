# 🚖 Ride-Hailing  Pipeline — PySpark & Azure Databricks
An end-to-end data engineering project that processes ride-hailing data using PySpark on Azure Databricks with incremental loading ,deduplication, and upsert operations.

##  Project Overview
This project simulates a real-world data pipeline for a ride-hailing platform.Raw data from multiple sources (customers, drivers, trips, payments, vehicles,locations) is ingested, cleaned, deduplicated, and loaded into a data warehouse using industry-standard ETL patterns.

## 🏗️ Architecture
Raw CSV Files (Data Lake)
        ↓
bronze Layer — Azure Databricks + PySpark
  Ingest raw data as-is
        ↓
Silver Layer — Azure Databricks + PySpark
  Clean → Deduplicate → Upsert → Incremental Load
        
## 🛠️ Tech Stack
| Tool | Purpose |
| Azure Databricks | PySpark processing environment |
| PySpark | Data transformations and processing |
| GitHub | Version control |




____________________________________ How to Use__________________________________________

### Prerequisites
-  Databricks workspace
- Python 3.x
- PySpark



_________________________________  Workflow Step By Step ___________________________________

STEP 1
----Create a catalogue in databrics
----Make a schema in the catalogue named source
----create a volume named source_data
----create directory for each csv file
----upload file in the corresponding volume


STEP 2
____Open Workspace
--Home --Folder -- creat a folder named Pyspark_project
--open a notebook -- name it Bronze_layer -- paste the code from "Bronze_ingestion" file
---Open another notebook -- name it silver_transformation --paste the code from  "silver_transformation" file


