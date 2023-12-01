# Sales-Analysis-Project

# 📝 Project Overview:
- Project Description: This project 📊 is a Power BI report that analyzes sales data. The goal is to gain insights from various aspects of the sales data by utilizing the Sales module, which contains information about sales orders, products, and sales territories.

# Data Transformation Plan:

## 1. Data Source and Connection:
  #### - File: 🗃️ CSV
  #### - Data Connectivity: 🔄 Import mode

## 2. Data Transformation Steps:
  #### 🛠️ a. Create Dimension Tables:
      - Identify the necessary dimensions: DimProduct, DimCustomer, DimGeography.
      - Create separate tables for each dimension, ensuring unique values for attributes.

   #### 🛠️ b. Create Date Dimension using M Language code:
      - Write M Language code to generate a date dimension table with date-related attributes.

   #### 🛠️ c. Split Columns by Delimiter:
      
  #### 🛠️ d. Remove Unnecessary Columns:
      - Identify and remove columns not relevant to the analysis.

   #### 🛠️ e. Rename Columns:
      - Make columns more descriptive and meaningful.

   #### 🛠️ f. Sort Table:
      - Arrange the data in the desired order by sorting the table.
![Screenshot 2023-12-01 164151](https://github.com/Othman5352/Sales-Analysis-Project/assets/140977589/3de5d794-fe31-4c52-9c0b-fb297767177a)


 #### 📊 b. Set Cardinality:
      - Define the type of relationship between tables (one-to-many).

   #### 📊 c. Optimize Performance:
      - Hide unnecessary columns to improve performance.

   #### 📊 d. Create a New Table to Organize Measures:
      - Create a separate table to organize calculated measures.
## 3. Data Modeling:
 #### 📊 a. Create Relations Between FactSales and Dimension Tables:
      - Establish relationships based on common attributes.
      - Crate star Schema.
![Screenshot 2023-12-01 163423](https://github.com/Othman5352/Sales-Analysis-Project/assets/140977589/3aef265f-63da-4f8a-bff8-606b5bb03134)


## 4. Calculated Measures:
  #### - Total Sales = SUM('FactOrders'[Unit Price]) 💰
  #### - Sales PY = CALCULATE([Total Sales], SAMEPERIODLASTYEAR(DimDate[Date])) ⏮️
   #### - Total Cost = SUM(FactOrders[Unit Cost]) 💸
   #### - Total Profit = [Total Sales] - [Total Cost] 💰💰💰
   #### - Profit Margin = DIVIDE([Total Profit], [Total Sales], 0) 📈
   #### - Total Transactions = COUNTROWS('FactOrders') 📊

## 5. Report Design:
### 🔍 Choose appropriate visualizations:
  #### - Line and Clustered Chart 📈
  #### - Stacked Bar Chart 📊
  #### - Card (New) 📄
  #### - Donut Chart 🍩
  #### - Clustered Bar Chart 📊
  #### - Clustered Column Chart 📊
  #### - Matrix Table 🗂️

   ### 🔍 Utilize Slicers for interactive filtering.

   ### 🔍 Incorporate buttons or page navigation for enhanced user experience.
![Screenshot 2023-12-01 163056](https://github.com/Othman5352/Sales-Analysis-Project/assets/140977589/848bfe2b-d845-409b-af64-637322f8ee87)

![Screenshot 2023-12-01 163315](https://github.com/Othman5352/Sales-Analysis-Project/assets/140977589/28160802-99c3-4bf8-b9c7-1a1cd792088d)


