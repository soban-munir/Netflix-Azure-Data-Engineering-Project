# Netflix-Azure-Data-Engineering-Project
End-to-End Azure Data Engineering Project using Azure Data Factory, Databricks, Delta Lake, and Power BI.

##  Project Overview  
This project demonstrates a **complete end-to-end Azure Data Engineering pipeline** integrating **Azure Data Factory (ADF)**, **Azure Databricks**, **Delta Lake**, and **Power BI**.  
The goal of this project is to build a **modern data lakehouse architecture** capable of **ingesting, transforming, and serving data for analytics** using a fully automated and parameterized workflow.

---

##  Architecture Overview  

### **Data Flow Summary:**
- **Source:** GitHub repository (raw data in JSON/CSV format)  
- **Ingestion:** Azure Data Factory pulls data from GitHub API and loads it into the **Bronze layer** of Azure Data Lake.  
- **Transformation:** Azure Databricks performs data cleaning and processing in the **Silver layer** using **Autoloader** for incremental ingestion.  
- **Data Modeling & ETL:** Delta Live Tables (DLT) are used in the **Gold layer** to create a refined, analytics-ready dataset.  
- **Visualization:** A Power BI connection is established using a **PBIDS (Power BI Data Source)** file, enabling analysts to visualize and explore the final data.

---

##  Key Features  

###  **Dynamic & Parameterized Pipelines:**  
- Designed **dynamic ADF pipelines** with **ForEach**, **If/Else**, and **Lookup** activities.  
- Replaced static notebooks with **parameterized Databricks notebooks**, making the pipeline reusable and scalable.  

###  **Incremental Data Ingestion:**  
- Implemented **Azure Databricks Autoloader** to automatically detect and process new files from the Data Lake.  
- Ensures efficient data ingestion with **schema evolution** support.  

###  **Delta Lake Architecture (Bronze → Silver → Gold):**  
- **Bronze Layer:** Raw data ingestion from GitHub API via ADF.  
- **Silver Layer:** Data cleansing, transformation, and normalization in Databricks.  
- **Gold Layer:** Created **Delta Live Tables** and ETL workflows to prepare high-quality analytical datasets.  

###  **End-to-End ETL Automation:**  
- Integrated **Azure Data Factory** with **Databricks** using Linked Services.  
- Automated scheduling and orchestration of all data movement and transformation jobs.  

###  **Power BI Integration:**  
- Generated **PBIDS (Power BI Data Source)** file to easily connect Power BI Desktop with the Gold layer dataset.  
- Enables Data Analysts to create dashboards using the refined and clean data.

---

##  Tech Stack  

| **Category** | **Tool/Service** |
|---------------|------------------|
| Cloud Platform | Microsoft Azure |
| Data Orchestration | Azure Data Factory |
| Data Processing | Azure Databricks (PySpark, Autoloader, Delta Live Tables) |
| Storage | Azure Data Lake Storage (Gen2) |
| Transformation Framework | Delta Lake Architecture (Bronze, Silver, Gold) |
| Visualization | Power BI |

---

##  Learning Outcomes  

- Built a **scalable and modular data pipeline** using Azure services.  
- Mastered **incremental ingestion** with **Databricks Autoloader**.  
- Created **reusable notebooks** and **dynamic ADF pipelines** for multi-table workflows.  
- Designed **Bronze–Silver–Gold architecture** following best practices.  
- Integrated data with **Power BI** for business-ready insights.

---

##  Future Improvements  

- Add **data quality checks** using *Great Expectations* or *Delta Expectations*.  
- Implement **Azure Synapse Analytics** for large-scale querying.  
- Automate deployment using **CI/CD (GitHub Actions + ADF Triggers)**.  
- Enable **real-time data streaming** using *Event Hubs* and *Databricks Structured Streaming*.

---

##  Author  

**👤 Soban Munir**  
📧 sobanmunir.official@gmail.com  
💼 https://www.linkedin.com/in/soban-munir  
