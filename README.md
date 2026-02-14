# 📊 Excel Power Query — Data Cleaning Assignment  
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Power Query](https://img.shields.io/badge/Power%20Query-0E6F9F?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-000000?style=for-the-badge&logo=github&logoColor=white)

This repository contains a **Power Query learning assignment** focused on cleaning, transforming, and preparing a real‑world sales dataset using **Excel + Power Query**.  
The project demonstrates a complete, professional data‑cleaning workflow — from handling messy dates to standardizing text fields — and documents each transformation step clearly.

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| **Sales_Records.xlsx** | Original raw dataset before any cleaning or transformations. |
| **sales_data_cleaned_power_query.xlsx** | Fully cleaned dataset after applying all Power Query steps. |

---

## 🎯 Project Purpose

This project was completed as part of a **Power Query learning assignment**, with the goal of practicing real‑world data cleaning techniques, improving data quality, and producing a reproducible workflow suitable for analytics and reporting.

---

## 🛠 Tools Used

- **Microsoft Excel**
- **Power Query (Get & Transform Data)**
- **GitHub** for version control and portfolio presentation

---

## 🔧 Data Cleaning Workflow (Power Query)

Below is the full, professional sequence of transformations performed on the dataset.

### **1. Load Raw Data**
- Imported the original Excel file into Power Query.

### **2. Trim & Clean Text Columns**
- Removed leading/trailing spaces.
- Removed hidden characters to ensure consistent formatting.

### **3. Standardize Text Casing**
- Converted names, regions, and product fields to **Capitalize Each Word**.

### **4. Replace Missing or Invalid Values**
- Replaced `NA`, `N/A`, blanks, and incorrect text entries with appropriate placeholders (e.g., “Unknown Customer”, “Unassigned”).
- Ensured no invalid text remained in numeric or date fields.

### **5. Fix Quantity Column**
- Converted written numbers (e.g., “five”, “three”) into numeric values.

### **6. Clean and Standardize the Date Column**
- Filtered out invalid entries (“Text”, nulls).  
- Replaced `-` with `/` to unify separators.  
- Used **Change Type Using Locale** to correctly interpret mixed date formats.  
- **No rows were manually deleted** — only filtered where necessary to maintain data integrity.

### **7. Change Data Types**
- Applied correct data types to all columns (Text, Whole Number, Decimal, Date).

### **8. Split Customer Name**
- Split full names into **First Name** and **Last Name** using the left‑most delimiter.

### **9. Standardize Region Values**
- Corrected inconsistent region labels (e.g., “east”, “EAST”, “East” → “East”).

### **10. Remove Nulls in Key Columns**
- Ensured essential fields (Order Date, Product, Quantity) contained no nulls.

### **11. Recalculate Total Sales**
- Added a custom column:  
  `Total Sales = Quantity * Unit Price`

### **12. Duplicate Handling**
- **Order ID was reviewed but NOT used as a unique key**, because multiple rows shared the same Order ID but contained different transaction details.  
- To preserve data accuracy, **no duplicate removal was performed**.

### **13. Load Cleaned Data**
- Loaded the final cleaned table back into Excel.

---

## 📈 Data Quality Summary

- **Total rows in raw dataset:** 101  
- **Rows filtered out due to invalid/missing dates:** 26  
- **Final cleaned dataset:** 75 rows  
- **Percentage filtered:** ~25.7%  
- All filtered rows were **unusable** and could not be repaired without guessing, ensuring data integrity.

---

## 🔁 Reproducibility

All cleaning steps are stored in the Power Query **Applied Steps** pane inside the cleaned Excel file.  
Anyone can reproduce the workflow by opening:

sales_data_cleaned_power_query.xlsx 
→ Data tab 
→ Queries & Connections 
→ Edit


---

## 📚 Learning Outcomes

Through this assignment, the following Power Query skills were practiced:

- Handling messy real‑world data  
- Cleaning and standardizing text fields  
- Fixing mixed date formats using **Using Locale**  
- Filtering invalid rows without manual deletion  
- Recalculating fields with custom formulas  
- Producing a clean, analysis‑ready dataset  
- Documenting a professional data‑cleaning workflow  
- Using GitHub for version control and portfolio building  

---

## 👤 Author

**Shaheen**  
Data Analyst (in training)  
Building strong foundations in Excel, Power Query, and reproducible data workflows.
