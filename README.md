# 💼 AtliQ Hardware – Global Sales Performance Analysis (Excel BI Project)

An **end-to-end Excel Business Intelligence (BI)** project analyzing **AtliQ Hardware’s global sales and profitability performance** across multiple fiscal years, customers, and markets.  

This project demonstrates how Microsoft Excel can be used as a **complete BI solution** — integrating **Power Query, Power Pivot, and DAX** to deliver interactive, data-driven dashboards for real business insights.

---

## 🎯 Project Objectives
- Build an integrated **Excel BI system** using Power Query, Power Pivot, and DAX.  
- Analyze **Net Sales, COGS, and Gross Margin %** across multiple fiscal years.  
- Evaluate **market-wise** and **customer-wise** profitability.  
- Compare **target vs actual performance** for global markets.  
- Deliver **interactive dashboards** to enable management-level decision-making.

---

## ⚙️ Workflow Overview

### 1️⃣ Data Preparation (Power Query)
- Imported raw sales data from multiple Excel sources.  
- Performed data cleaning — handled blanks, renamed columns, removed duplicates.  
- Standardized fiscal periods and markets for consistency.  
- Created a **custom Date Table** with calculated columns for:
  - Fiscal Year  
  - Fiscal Month  
  - Month Order  
  - Month Name  

> ⚙️ *Note:* Source connections are disabled in this version for portability.  
> The final Excel model reflects all applied transformations.

---

### 2️⃣ Data Modeling (Power Pivot)
Developed a **Star Schema** model connecting fact and dimension tables:  

| Fact Table | Dimension Tables |
|-------------|------------------|
| `Sales_Fact` | `dim_customer`, `dim_market`, `dim_product`, `dim_date` |

Relationships established on:
- `Customer Code`  
- `Product Code`  
- `Market`  
- `Date`

---

### 3️⃣ DAX Measures
Created custom measures using **DAX** for advanced financial insights:  
- **Net Sales** = `SUM(Sales[Net_Sales])`  
- **Gross Margin** = `[Net Sales] - [COGS]`  
- **GM %** = `DIVIDE([Gross Margin], [Net Sales], 0)`  
- **Net Sales FY21 / FY22 / FY23** using `CALCULATE()` with filter context  

---

### 4️⃣ Dashboard Design
Developed four interactive dashboards showcasing different business perspectives:

#### 📆 Fiscal Year Analysis  
> P&L report tracking Net Sales, COGS, and GM% across fiscal months.  
![Fiscal View](Screenshots/Fiscal_Year_Analysis.png)

---

#### 🌍 Market Insights  
> Regional profitability comparison with visual heatmaps.  
![Market View](Screenshots/Market_Analysis.png)

---

#### 👥 Customer Performance  
> Year-over-year sales growth and contribution of top customers.  
![Customer View](Screenshots/Customer_Performance.png)

---

#### 🎯 Market vs Target Performance  
> Compares actual performance vs yearly targets for each market.  
![Target View](Screenshots/Sales_Performance.png)

---

## 📊 Key Insights
- **India**, **USA**, and **Canada** are the top-performing markets.  
- **Gross Margin %** remains consistent around 41–42%, showing healthy profitability.  
- Certain regions underperformed due to rising costs and COGS inefficiency.  
- **AtliQ Exclusive** and **Croma** exhibited the strongest YoY growth.  

---

## 🧩 Tools & Technologies Used

| Tool | Purpose |
|------|----------|
| **Microsoft Excel** | Core analytics and reporting platform |
| **Power Query** | ETL – data extraction, transformation, and loading |
| **Power Pivot** | Data modeling and relationship management |
| **DAX** | Custom KPIs and time intelligence |
| **Conditional Formatting & Slicers** | Interactive visualization and storytelling |

---

## 📈 Learnings
- Structured an **end-to-end Excel BI workflow** combining data cleaning, modeling, and visualization.  
- Practiced creating **custom DAX measures** for financial and time-based analytics.  
- Learned how to apply **data modeling principles (Star Schema)** inside Excel.  
- Designed **executive-level dashboards** for data storytelling and strategic insights.

---

## 📁 Project Files

| File | Description |
|------|--------------|
| `Global_Sales_Fiscal.xlsx` | Fiscal Year P&L Dashboard |
| `Global_Sales_Market.xlsx` | Market-wise profitability analysis |
| `Global_Sales_Customers.xlsx` | Customer performance report |
| `Global_Sales_Target.xlsx` | Market vs Target dashboard |

🔗 [Download Excel Project (Google Drive)](https://drive.google.com/file/d/1bzLO7r_hEFuCKO1pAWbwLHdYQxUnkVHB/view?usp=sharing)

---

## 🧠 Data Model (Power Pivot)
Star Schema built with Fact and Dimension tables linked through keys (Customer, Product, Market, Date).  

![Data Model](Screenshots/Data_Model.png)

---

## 👨‍💻 About Me
I’m **Yash Hooda**, an aspiring **Data Analyst** skilled in **Power BI, Excel, and SQL**.  
Passionate about transforming complex datasets into meaningful stories through data modeling and visualization.

📍 *Rohtak, Haryana, India*  
📫 **yash111vision@gmail.com**  
🌐 [GitHub](https://github.com/11Yash1) | [LinkedIn](https://www.linkedin.com/) *(coming soon)*  

---

⭐ *If you found this project interesting, don’t forget to star the repository!*  

---

## 💡 Why This Project Stands Out
- Demonstrates **Excel as a full BI environment** – ETL, modeling, DAX, and visualization in one tool.  
- Uses **real financial data** for multi-year performance insights.  
- Reflects **enterprise-style dashboards** similar to those used by consulting firms (Deloitte, PwC, KPMG).  
- Proves ability to **design and communicate insights** clearly with advanced Excel features.  
