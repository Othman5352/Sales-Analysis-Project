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
