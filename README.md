# ⚽ European Football Transfer Market Analysis (2009–2021) | Power BI Report

## 📌 Project Overview

This project analyzes the European football transfer market using Power BI.

It demonstrates a complete end-to-end Business Intelligence workflow including:

- Data cleaning in Power Query
- Transformation of raw dataset
- Star schema data modeling
- Creation of calculated columns & DAX measures
- Interactive multi-page dashboard
  
The objective was to convert raw football transfer data into decision-ready insights.

## 🧹 Data Cleaning & Transformation (Power Query)

The dataset required extensive preprocessing before analysis.

### ✔ Cleaning Steps Performed

- Promoted headers for structured dataset
- Corrected data types for numeric & categorical fields
- Renamed columns for consistency
- Removed unnecessary columns
- Reordered columns for model clarity
- Filtered invalid and null records
- Standardized text values across leagues, teams, and players

### ✔ Transformation Steps Implemented

The following transformations were applied:

- Multiple Replace Value operations to fix inconsistent text and missing entries
- Several Filtered Rows steps to remove invalid transfers
- Renamed Columns (multiple stages) to align with dimensional modeling
- Changed Data Types for proper aggregation
- Reordered Columns for structured schema building
- Removed Other Columns to keep only relevant features

These steps ensured the dataset was clean, consistent, and analysis-ready.

## 🏗 Data Modeling (Star Schema)

A professional star schema was created for performance and scalability.

### ⭐ Fact Table:

Fact_Transfer

Contains transactional transfer data:

- Transfer Fee
- Market Value
- Season
- Window
- Player ID
- Team ID
- Loan / Free / Retired indicators

### 🌐 Dimension Tables:

1] Dim_Player

- Player Name
- Age
- Position
- Nationality

2] Dim_Team
- Team Name
- League
- Country

3] Dim_CounterTeam

- Counter team details for transfer direction tracking

This model allows:

- Faster queries
- Cleaner relationships
- Realistic enterprise BI structure

## 🧮 DAX Implementation

### ✔ Measures Created

- Total Transfers
- Average Transfer Fee
- Average Market Value
- Total Loan Transfers
- Total Free Transfers
- Total Ongoing Loans
- Total Ended Loans
- Top Market Value KPI

### ✔ Calculated Columns Created

- Loan Status classification
- Player Type categorization
- Transfer Type logic
- Retired Type classification
- Season grouping
- Free / Loan / Retired flags

These calculations helped transform raw data into business KPIs.

## 📊 Dashboard Structure

### 1️⃣ Overview Page

- Total Transfers: 69.99K
- Avg Transfer Fee: €3.76M
- Market value indicators:
1] Seasonal transfer trends
2] Incoming vs outgoing comparison
3] Player activity insights

### 2️⃣ League Analysis Page

- Market value comparison by league
- Transfer spending by league
- League ranking visuals
- Financial dominance insights

### 3️⃣ Transfer Analysis Page

- Permanent vs Loan breakdown
- Paid vs Free transfer analysis
- Loan lifecycle tracking
- Top countries spending
- Top clubs spending

### 4️⃣ Player Performance Analysis Page

- Top players by market value
- Highest transfer fee players
- Position distribution
- Player demand by age curve

Key insights:

- Peak transfer demand: 20–27 years
- Average player age: 23
- Retirement age: 31

### 5️⃣ Conclusion Page

Final insights derived:

- Elite leagues dominate financially
- Loan transfers used as risk-control strategy
- Young players provide highest long-term value
- Smaller leagues function as talent suppliers

## 🛠 Tools & Technologies Used

- Power BI
- Power Query (ETL & Cleaning)
- DAX (Measures & Calculated Columns)
- Star Schema Modeling
- Kaggle Dataset

## 📂 Dataset Source

The dataset used in this project was obtained from Kaggle.

🔗 Dataset Link:
https://www.kaggle.com/datasets/mexwell/football-transfer-dataset?utm_source=chatgpt.com

 ## Author

### Neha Jadhav
Aspiring Data Analyst

## ⭐ If You Like This Project

- Star this repository
- Share feedback
