📊 Data Analysis Project – Sales & Customer Insights
🧹 Data Cleaning
No duplicate records were found; however, inconsistencies were identified and resolved.
Sheet 1:
Cleaned Customer ID and Country using Find & Replace.
Fixed Customer Name formatting using:
TRIM() → removed extra spaces
PROPER() → capitalized names properly
Sheet 2:
Standardized Product ID using Find & Replace.
🔄 Data Imputation

Loyalty Level (Sheet 1):

=IF(ISBLANK(cell), "Unknown", cell)
Replaced missing values with "Unknown"

Cost & Stock Columns:

=IF(ISBLANK(cell), AVERAGEIF(range, criteria, average_range), cell)
Filled missing values using subcategory-wise averages
Sales Fact Table (Sheet 4):

Unit Price:

=IF(ISBLANK(Unit_Price), Total_Amount / (Qty * (1 - Discount)), Unit_Price)

Discount:

=IF(ISBLANK(Discount), 1 - (Total_Amount / (Qty * Unit_Price)), Discount)
Established relationships across sheets using VLOOKUP for integrated analysis.
Used Data Analysis ToolPak to calculate:
Sum, Average, Median, Mode, Skewness
Applied on Quantity and Total Price
📈 Pivot Tables & Visualizations
Built interactive dashboards using PivotTables and charts:
📅 Month-wise & Year-wise Total Sales
🛍️ Category-wise Sales Count
🏬 Store Type-wise Sales Count
👩‍🦰👨 Gender vs Category Analysis
🔝 Top 10 Products by Sales
🎛️ Added a common slicer for dynamic filtering across all visuals
🔍 Key Insights
👩 Female customers contributed the majority of purchases
🌍 North Region recorded the highest sales
🛒 Online stores generated the largest share of revenue
🏅 Sports category is the most popular among all customers
🛠️ Tools & Technologies
Microsoft Excel
Pivot Tables & Charts
Data Analysis ToolPak
Functions: TRIM(), PROPER(), IF(), ISBLANK(), AVERAGEIF(), VLOOKUP()
📌 Conclusion

This project demonstrates effective data cleaning, transformation, and analysis using Excel to generate meaningful business insights and interactive dashboards.<img width="1012" height="451" alt="Dashboard Report" src="https://github.com/user-attachments/assets/4dd0439b-edfd-4f21-8aba-a7f77755d62e" />
