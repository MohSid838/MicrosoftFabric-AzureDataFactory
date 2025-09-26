# 🚀 Sales Analytics Project (Microsoft Fabric + Azure Data Factory+PowerBI)

This project demonstrates how to build a complete **Sales Data Platform** using **Microsoft Fabric, Azure Data Factory (ADF), Data Warehouse, and Power BI**.

---

## 📂 Project Workflow

### 1️⃣ Create Sales Lakehouse
- Set up a **Lakehouse** named `Sales_Lakehouse`.
- Acts as the **staging and storage layer** for raw and transformed data.

---

### 2️⃣ Build Sales Pipeline (Using Azure Data Factory)

Steps included in the pipeline:
1. **Delete Activity** → Remove existing files from `Sales_Lakehouse` before every fresh load.  
2. **Copy Activity** → Extract Sales data from **API** and load it into `Sales_Lakehouse`.  
3. **Transformations**:  
   - Use a **Notebook** for advanced transformations.  
   - Alternatively, use a **Dataflow** for low-code/no-code transformations.  
4. **Scheduling** → Configure the pipeline to run **daily** for automated refresh.  

---

### 3️⃣ Create Sales Data Warehouse (Sales_DWH)

1. Create a **Sales schema** inside the Data Warehouse.  
2. Define **Dimension and Fact tables**:  
   - `Dim_Customer`  
   - `Dim_Item`  
   - `Fact_Sales`  
3. Implement a **Stored Procedure** to load transformed data from `Sales_Lakehouse` into `Sales_DWH`.  

---

### 4️⃣ Build Semantic Model
- Create a **semantic model** in Fabric.  
- Add relationships, hierarchies, and KPIs for meaningful reporting.  

---

### 5️⃣ Develop Power BI Report (Sales_Dashboard)
- Connect Power BI to the **semantic model**.  
- Build a **Sales Dashboard** with key insights:  
  - 📊 Sales by Customer  
  - 📦 Sales by Item  
  - 📈 Sales Trends (Year, Month, Day)  
  - 💰 Tax & Revenue insights  

---

## 🔗 Reference GitHub Repository
👉 [MicrosoftFabric-AzureDataFactory Project](https://github.com/MohSid838/MicrosoftFabric-AzureDataFactory/tree/main/1.%20Project%20-%20Sales%20Pipeline)

---

## ⚡ Tech Stack
- **Microsoft Fabric** → Lakehouse, Data Warehouse, Semantic Model  
- **Azure Data Factory** → Pipelines, Dataflows, Scheduling  
- **Power BI** → Reporting & Visualization  
- **SQL & Notebooks (PySpark/Python)**  

---

## 📌 Future Enhancements
- Add monitoring & logging for ADF pipelines.  
- Extend pipeline to support **incremental data loads**.  
- Enhance dashboard with **predictive analytics**.  
