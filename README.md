# Customer-Analysis Dashboard Using Tableau

This project involves building an interactive Tableau dashboard to analyze customer revenue patterns based on various dimensions like month, age group, state, category, discount correlation, and region. The goal is to provide a comprehensive visual insight into revenue distribution and customer behavior.
<br>
Data Modeling:
<br>
Objective:
<br>
Structure raw data into meaningful tables and relationships, ensuring smooth analysis.
- **Source Data:
   - **The data was imported from a CSV/Excel file containing sales transaction records, including fields like Order Date, Revenue, State, Age, Category, Region, Discount %, Quantity Ordered, Gender, etc.
- **Model Structure:
   - **The dataset was treated as a flat file model (single table).
   - **All columns were reviewed and assigned correct data types (Date, String, Integer, Decimal).
- **Created calculated fields:
   - **Revenue per Month = SUM of Revenue grouped by month (from Order Date).
   - **Revenue per State = SUM of Revenue grouped by State.
   - **Revenue per Age Group = Bucketed Age into groups (<20, 20-30, etc.).
   - **Revenue Percentage per Region = Percent of total revenue by Region.
   - **Quantity Discount Correlation = Correlation analysis between Discount % and Quantity Ordered.
   - **Revenue per Category by Gender = Split revenue into Female & Male categories.

Analysis and create a dashboard report.
