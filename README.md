---

# 📊 Sales & Customer Insights Dashboard

![Excel](https://img.shields.io/badge/Tool-Excel-green)
![Data Analysis](https://img.shields.io/badge/Focus-Data%20Analysis-blue)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

---

## 📌 Project Overview

This project focuses on analyzing **sales and customer data** to uncover meaningful business insights.
The workflow includes **data cleaning, data imputation, transformation, and visualization** using Microsoft Excel.

---

## 🧹 Data Cleaning

* Verified dataset integrity — **no duplicate records found**
* Resolved inconsistencies across multiple sheets:

  * Cleaned *Customer ID* and *Country* using **Find & Replace**
  * Standardized *Customer Name* using:

    * `TRIM()` → removed extra spaces
    * `PROPER()` → formatted names properly
  * Fixed *Product ID* inconsistencies in Sheet 2

---

## 🔄 Data Imputation

Handled missing values using logical and statistical methods:

* **Categorical Data (Loyalty Level):**

  ```excel
  =IF(ISBLANK(cell), "Unknown", cell)
  ```

* **Numerical Data (Cost, Stock):**

  ```excel
  =IF(ISBLANK(cell), AVERAGEIF(range, criteria, average_range), cell)
  ```

  ✔ Filled values using **subcategory-based averages**

* **Sales Fact Table Adjustments:**

  * **Unit Price:**

    ```excel
    =IF(ISBLANK(Unit_Price), Total_Amount / (Qty * (1 - Discount)), Unit_Price)
    ```
  * **Discount:**

    ```excel
    =IF(ISBLANK(Discount), 1 - (Total_Amount / (Qty * Unit_Price)), Discount)
    ```

* Integrated datasets using **VLOOKUP** for relational mapping

* Performed statistical analysis using **Data Analysis ToolPak**:

  * Sum | Average | Median | Mode | Skewness

---

## 📈 Dashboard & Visualizations

Built an interactive Excel dashboard with:

* 📅 **Sales Trend Analysis** (Month-wise & Year-wise)
* 🛍️ **Category-wise Sales Distribution**
* 🏬 **Store Type Performance**
* 👥 **Gender-based Purchase Analysis**
* 🔝 **Top 10 Performing Products**

🎛️ **Interactive Feature:**

* Unified **Slicer** for dynamic filtering across all charts

---

## 🔍 Key Insights

* 👩 Female customers drive **higher purchase volume**
* 🌍 North Region leads in **overall sales performance**
* 🛒 Online stores contribute the **largest revenue share**
* 🏅 Sports category is the **top-performing segment**

---

## 🛠️ Tools & Skills Used

* **Microsoft Excel**
* Pivot Tables & Charts
* Data Analysis ToolPak
* Data Cleaning & Transformation
* Functions:

  ```
  TRIM(), PROPER(), IF(), ISBLANK(), AVERAGEIF(), VLOOKUP()
  ```

---

## 📷 Dashboard Preview

> *(Add your dashboard screenshots here for better presentation)*

---

## 📌 Conclusion

This project highlights the ability to:

* Clean and preprocess raw data
* Handle missing values effectively
* Build interactive dashboards
* Derive actionable business insights

---
<img width="1012" height="451" alt="Dashboard Report" src="https://github.com/user-attachments/assets/ecf8718f-f0ef-4ffc-8a6c-cca2bbc8ef26" />


