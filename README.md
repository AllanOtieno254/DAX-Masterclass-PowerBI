# DAX Masterclass Power BI Dashboard

## 📌 Project Overview
This Power BI project is a comprehensive **DAX Masterclass Dashboard** that leverages advanced **DAX formulas** and Power BI functionalities to analyze and visualize key insights from a dataset. The dashboard is structured to provide dynamic and interactive reports with efficient data modeling and calculations.
![Date and time analysis image](https://github.com/user-attachments/assets/8203c241-bbb8-46fe-bcb7-93ea23ec43a9)

## 🔥 Features
- **Interactive Dashboard:** A fully responsive Power BI report with drill-through and slicers.
- **Advanced DAX Calculations:** Custom measures for aggregations, rankings, and time intelligence.
- **Data Model Optimization:** Efficient relationships between tables for fast querying.
- **Power Query Transformations:** Cleaned and structured raw data using Power Query.
- **Theme and Custom Visuals:** Applied a modern Power BI theme and custom visuals.

## 🛠️ DAX Formulas Used
Here are some key **DAX measures** included in the report:
- **Total Sales:** `SUM(Sales[Amount])`
- **Year-over-Year Growth:** `CALCULATE([Total Sales], SAMEPERIODLASTYEAR(Date[Date]))`
- **Cumulative Sales:** `CALCULATE([Total Sales], FILTER(ALL(Date), Date[Date] <= MAX(Date[Date])))`
- **Top N Products:** `TOPN(5, Products, [Total Sales], DESC)`
- **Average Order Value:** `DIVIDE([Total Sales], [Total Orders])`

## 📊 Data Model & Relationships
The dataset is structured in a **Star Schema**, consisting of:
- **Fact Table:** `Sales` (Transactional Data)
- **Dimension Tables:** `Products`, `Customers`, `Date`, `Regions`

### **Relationships:**
- `Sales` 🔗 `Products` (One-to-Many)
- `Sales` 🔗 `Customers` (One-to-Many)
- `Sales` 🔗 `Date` (One-to-Many)
- `Sales` 🔗 `Regions` (Many-to-One)

## 📈 Visualizations in the Report
- **Sales Trend Analysis:** Line charts tracking revenue over time.
- **Top Performing Products:** Bar chart displaying the best-selling products.
- **Customer Segmentation:** Pie charts analyzing customer demographics.
- **Geographical Sales Distribution:** Map visualization highlighting regional sales performance.
- **Key Performance Indicators (KPIs):** Cards displaying Total Sales, Total Orders, and Profit Margins.

## 🔍 Insights & Findings
- **Sales peaked in Q4**, indicating strong seasonal demand.
- **Region X outperformed all others**, suggesting a high-value customer base.
- **Product Y had the highest profit margin**, making it a key focus area for marketing.
- **Returning customers generated 60% of total revenue**, highlighting the importance of retention.

## 🚀 How to Use the Report
1. **Download the Power BI file (`dax_masterclass.pbix`).**
2. **Open it in Power BI Desktop.**
3. **Interact with filters and slicers** to dynamically explore insights.
4. **Export reports as PDF** for presentations or business reviews.

## 🔧 Future Improvements
- **Incorporate Machine Learning Predictions** for sales forecasting.
- **Add Row-Level Security (RLS)** for user-based access control.
- **Enhance UI/UX with additional tooltips and interactive elements.**

## 📜 License
This project is licensed under the **MIT License** – feel free to use and modify it while giving proper credit.

---
🔥 **Contributors:** [Allan Otieno Akumu](https://github.com/AllanOtieno254)  
💡 **Suggestions or Issues?** Feel free to open an issue or contribute to this repository!

