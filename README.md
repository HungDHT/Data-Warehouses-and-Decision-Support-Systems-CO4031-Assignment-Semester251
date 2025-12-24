### 🚀 Project Overview
This project is a full-stack **Decision Support System (DSS)** designed to transform raw transactional data from the CompanyX database into actionable marketing insights. It implements a 3-Tier BI Architecture to enable **Behavioral Segmentation**, **Profitability Analysis**, and automated **Marketing Recommendations**.

### 🏗️ Architecture & Tech Stack
* **Database (SQL Server):** Designed a Star Schema Data Warehouse (`FactSales`, `DimCustomer`, etc.) optimized for analytical queries.
* **ETL (SSIS):** Developed robust packages to extract, clean, and load data.
* **Semantic Layer (SSAS Tabular):** Built a centralized logic model using DAX to calculate KPIs (Profit, Margins) and implement row-level segmentation.
* **Visualization (Power BI):** Created an interactive dashboard connected "Live" to SSAS, featuring "What-If" analysis and tactical customer lists.

### 💡 Key Features
* **Behavioral Segmentation:** Classifies customers into **Gold, Silver, and Bronze** tiers based on actual Lifetime Spend rather than static demographics.
* **Profitability Focus:** Goes beyond revenue to calculate **True Profit**, identifying high-revenue customers who are actually unprofitable due to costs/returns.
* **The "Action Engine":** A custom DAX logic engine that automatically evaluates every customer and assigns a **Next Best Action** (e.g., *"🚨 Flag: Unprofitable"*, *"⭐ Upsell to Gold"*, or *"💎 Reward VIP"*).
* **Tactical Command Center:** A Power BI interface designed for operations teams to generate targeted call lists based on specific strategies.

### 📂 Repository Structure
* `/Database`: SQL scripts for generating the Data Warehouse schema.
* `/SSIS_ETL`: Visual Studio integration services packages.
* `/SSAS_Model`: The Tabular Model project including DAX measures.
* `/PowerBI_Report`: The final `.pbix` dashboard file.
* `Project_Report.pdf`: Detailed documentation of the design and implementation.
