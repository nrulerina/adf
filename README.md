# 🚀 Azure Data Factory - Parametrized Pipeline Project

This project demonstrates how to build a **parametrized pipeline in Azure Data Factory (ADF)** to move CSV data from Azure Blob Storage into an Azure SQL Database using a dynamic and reusable data flow.

![Architecture](./Screenshot%202025-04-10%20140011.png)

---

## 📌 Project Overview

This solution ingests `.csv` files (`Cars.csv` and `Planes.csv`) stored in Azure Blob Storage and loads the data into corresponding SQL tables (`Cars Table` and `Planes Table`) using a single, parameterized pipeline in Azure Data Factory.

---

## ⚙️ Architecture Breakdown

1. **Source Storage**  
   - Azure Blob Storage with files:  
     - `Cars.csv`  
     - `Planes.csv`

2. **Azure Data Factory Components**  
   - **Linked Services**: for Blob Storage & Azure SQL  
   - **Parametrized Datasets**: dynamic input/output  
   - **Parametrized Pipeline**: single pipeline for multiple datasets  
   - **Copy Activity**: to move data

3. **Target Storage**  
   - Azure SQL Database with tables:  
     - `Cars` table  
     - `Planes` table

---

## 🔁 Workflow Description

1. The ADF pipeline is triggered with parameters (e.g., `fileName`, `TableName`).
2. Based on these parameters:
   - It reads the specified CSV from Blob Storage.
   - Writes the data to the correct SQL table.
3. The same pipeline logic is reused for different datasets using different parameter values.

📌 Note: This project is part of my personal learning journey and was built by referring to a YouTube tutorial.
Credit goes to the original creator for helping me understand Azure Data Factory concepts clearly.
I highly recommend using YouTube as a powerful tool to explore cloud and data engineering skills.


