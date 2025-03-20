# Customer-Analysis Dashboard Using Tableau

This project involves building an interactive Tableau dashboard to analyze customer revenue patterns based on various dimensions like month, age group, state, category, discount correlation, and region. The goal is to provide a comprehensive visual insight into revenue distribution and customer behavior.
<br>
Data Modeling:
<br>
Objective:
<br>
Structure raw data into meaningful tables and relationships, ensuring smooth analysis.
- **Source Data:**
   - **The data was imported from a CSV/Excel file containing sales transaction records, including fields like Order Date, Revenue, State, Age, Category, Region, Discount %, Quantity Ordered, Gender, etc.**
- **Model Structure:**
   - **The dataset was treated as a flat file model (single table).**
   - **All columns were reviewed and assigned correct data types (Date, String, Integer, Decimal).**
- **Created calculated fields:**
   - **Revenue per Month = SUM of Revenue grouped by month (from Order Date).**
   - **Revenue per State = SUM of Revenue grouped by State.**
   - **Revenue per Age Group = Bucketed Age into groups (<20, 20-30, etc.).**
   - **Revenue Percentage per Region = Percent of total revenue by Region.**
   - **Quantity Discount Correlation = Correlation analysis between Discount % and Quantity Ordered.**
   - **Revenue per Category by Gender = Split revenue into Female & Male categories.**

Data Cleaning:
Objective:Ensure clean, consistent, and error-free data for accurate visualization.
- **Removed null/blank values in critical columns like Revenue, State, Category.**
- **Standardized column names (renamed for readability).**
- **Filtered out rows with missing or unknown values (e.g., states with “Unknown” were highlighted in the map for transparency).**
- **Corrected inconsistent entries in Region and Category columns (e.g., ensuring categories like "Mobiles & Tablets" are uniformly labeled).**
- **Ensured date formats were consistent (MM-DD-YYYY).**

Data Processing:
Objective:
Prepare the data by aggregating, transforming, and filtering as needed.
- **Aggregated revenue data:**
   - **Monthly Aggregation: Used DATEPART function to group revenue by month.**
   - **Age Group Aggregation: Created calculated fields to bucket ages.**
   - **Region & State Aggregation: Grouped revenue by geographic regions and states.**
   - **Gender Split Aggregation: Filtered revenue by gender to analyze category-wise male vs female revenue.**
- **Applied filters & parameters:**
   - **Added Category Filter Dropdown for dynamic filtering.**
- **Applied Sort & Rank to visualize categories based on revenue.**
- **Used calculated fields for Revenue Percentages & Totals.**

 Data Visualization:
Objective:
Create interactive, insightful, and user-friendly visualizations.

**Dashboards & Charts Created:**

- 1.Revenue Per Month (Line Chart):
    - **Displays month-wise revenue trend.**
    - **Highlights peak sales months (e.g., October ₹11.5M).**
- 2.Revenue Per State (Map):
    - **Geographical visualization showing revenue distribution across US states.**
- 3.Revenue Based on Age (Bar Chart):
    - **Visualizes revenue contribution by age groups (e.g., highest from 30-40 age group ₹8.7M).**
- 4.Revenue Percentage Per Region (Donut Chart):
    - **Shows revenue percentage breakdown by region (e.g., South contributes 36.83%).**
- 5.Quantity Discount Correlation (Scatter Plot):
    - **Shows relationship between Discount % and Quantity Ordered.**
- 6.Revenue Per Category (Bar Chart - Split by Gender):
    - **Displays revenue distribution across product categories.**
    - **Split view of Male & Female contributions (e.g., Mobiles & Tablets ₹11.4M for Female, ₹10.8M for Male).**
- 7.Total Revenue (KPI Metric):
    - **Displays overall revenue (₹41.7M).**
 
Dashboard Interaction <a href="https://github.com/Moinkhan123456/Customer-Analysis/blob/main/Screenshot%20(8).png">View Dashboard</a>
<br>
Analysis and create a dashboard report.
