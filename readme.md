# Azure Data Engineering Project (ADF + SQL + ADLS + MEDALLION Architecture)

## Project Architecture
<img width="1041" height="659" alt="image" src="https://github.com/user-attachments/assets/d67219ed-2b58-42a7-8876-9a8e5d4759e5" />

## Dynamic Pipeline Visuals
<img width="1041" height="314" alt="image" src="https://github.com/user-attachments/assets/4603cbc6-c436-4dc8-b10e-6dd1c30dc422" />
<img width="790" height="311" alt="image" src="https://github.com/user-attachments/assets/9e2521f7-8196-42f4-83a6-4cd27e435529" />
<img width="1134" height="150" alt="image" src="https://github.com/user-attachments/assets/fabbe53a-79f3-4a03-829e-a1e1893fde80" />

## Project Overview
This project demonstrates an end-to-end **Azure Data Engineering pipeline** using **Azure Data Factory (ADF)**.  
It ingests data from multiple sources, performs processing, and loads data into a target system for analytics using **Medallion Architecture**.

---

## Tech Stack
- Azure Data Factory (ADF)
- Azure SQL Database
- Azure Data Lake Storage Gen2 (ADLS)
- GitHub (ADF Git integration)
- Web Activity / Logic App (for failure alerts)

---

## High Level Flow
1. Bronze ingestion (raw data load)
2. API ingestion
3. SQL → Data Lake copy (incremental load)
4. Failure alert trigger (on pipeline failure)
5. Silver Layer with various data transformations
6. Gold layer with buisness ready logics & insights

---

## Repository Structure
- `pipeline/` → ADF pipelines  
- `dataset/` → Datasets (source/target definitions)  
- `linkedService/` → Connections (SQL/ADLS/API)  
- `integrationRuntime/` → Integration runtime configuration  
- `dataflow/` → Mapping data flows (if used)  
- `factory/` → Factory settings  

---

## Key Features
- Incremental data load
- ForEach activity for dynamic processing
- Error handling + failure alert
- GitHub version control (main + adf_publish)

---

## Git Workflow
- Collaboration branch: `main`
- Publish branch: `adf_publish`

---

## Author
**Rohan Dubey**
