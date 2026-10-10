# 🛍️ Maven Market Sales Performance Dashboard

An interactive **Power BI dashboard** built on a multi-table **star schema** to track revenue, profit, transactions, and returns for **Maven Market**, a multi-country grocery retailer, against monthly goals and targets.

---

## 📌 Project Overview

**Purpose:** To combine sales, product, store, region, customer, and returns data into one data model and dashboard, so a business can monitor topline performance, compare results with goals, and find which brands, stores, and cities drive revenue and returns.

**Key questions answered:**
- How much revenue, cost, and profit is the business generating, and what is the profit margin?
- Is the current month on track against its transaction, profit, and returns goals?
- Is weekly revenue meeting its target?
- Which product brands have the strongest profit margins and highest return rates?
- How do transactions vary by store city and country (USA, Canada, Mexico)?

---

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Data Visualization | Power BI Desktop |
| Data Modeling | Star schema with 1-to-many relationships |
| Calculations & KPIs | DAX (time intelligence, goals, ratios) |
| Data Preparation | Power Query |

---

## 📂 Data Source

- **Dataset:** Maven Market retail sample data (Maven Analytics), covering **1997–1998**
- **Tables (7):**

| Table | Type | Key fields |
|---|---|---|
| **Transactions** | Fact | customer_id, product_id, store_id, stock_date, transaction_date |
| **Returns_1997-1998** | Fact | product_id, store_id, return_date |
| **Products** | Dimension | product_id, product_name, product_brand, product_cost, product_retail_price, discount_price, low_fat, Price_Tier |
| **Stores** | Dimension | store_id, store_name, store_city, store_country, region_id, grocery_sqft, first_opened_date, last_remodel_date |
| **Regions** | Dimension | region_id, sales_district, sales_region |
| **Customers** | Dimension | customer_id |
| **Calendar** | Dimension | date, Day Name, Month Name, Quarter, Start of Week, Start of Month, End of Month |

- **Source link:** *(add the dataset link here)*

---

## ⚙️ Project Workflow

1. **Data Import & Cleaning:** Loaded the tables into Power BI and prepared them in Power Query.
2. **Data Modeling:** Connected fact tables (Transactions, Returns) to dimension tables (Products, Stores, Regions, Customers, Calendar) in a star schema.
3. **DAX Measures:** Created measures for revenue, cost, profit, profit margin, return rate, goals, targets, and time-based calculations.
4. **Dashboard Design:** Built a multi-page report with goal-based KPI cards, a conditional-formatting table, a map, and trend charts.
5. **Insights:** Analyzed performance against goals and targets across brands, stores, and cities.

---

## 📊 Dashboard Pages

| Page | What it shows |
|---|---|
| **Topline Performance** | Current-month KPI cards against goals, brand performance table, transactions by store city on a map, country slicer, weekly revenue trend, revenue vs target gauge |
| **KPI Measures (regions)** | Full set of business KPIs: quantity sold, returns, revenue, cost, profit, margin, weekend transactions, revenue target, 60-day revenue, last-month figures, and YTD revenue |
| **Notes** | Project notes and documentation |

---

## ✨ Features

- **Goal-based KPI cards** for Current Month Transactions, Profit, and Returns, each showing the goal and the percentage difference
- **Brand performance table** with Total Transaction, Total Profit, Profit Margin, and Return Rate, using data bars and color scales
- **Interactive map** of transactions by store city, with a country slicer (USA, Canada, Mexico)
- **Weekly Revenue Trending** column chart
- **Revenue vs Target** gauge
- **Time intelligence** measures: YTD revenue, 60-day revenue, and last-month comparisons
- **Star schema model** with a dedicated Calendar table

---

## 🔍 Key Insights

- The business generated about **$1.76M** in revenue at a cost of about **$0.71M**, leaving about **$1.05M** in profit, a **59.67% profit margin**.
- About **833K units** were sold across **270K transactions**, covering **1.56K unique products**.
- The **return rate is low, about 0.99%**, from about 8.3K units returned.
- About **28.4%** of transactions happen on weekends.
- The current-month cards compare actual performance to goals, for example transactions of 2,225 against a goal of 2,221.

---

## 🌟 Highlights

- Built a **7-table star schema** with fact and dimension tables
- Created **DAX measures** for revenue, profit, margin, return rate, goals, and time intelligence
- Combined **goal tracking** and **target comparison** in one view
- Used **conditional formatting** to spot high-margin and high-return brands quickly
- Designed for business stakeholders to monitor performance at a glance

---

## 🖼️ Screen Shots
![Topline Performance](images/topline_performance.png)
![KPI Measures](images/kpi_measures.png)
![Data Model](images/data_model.png)

---

## 📁 Repository Structure

```
Maven-Market-Dashboard/
│
├── Maven_Market_Dashboard.pbix    # Power BI file
├── images/                        # Dashboard and data model screenshots
└── README.md
```

---

## 🚀 How to Use

1. Download or clone this repository.
2. Open the `.pbix` file in **Power BI Desktop**.
3. Use the country slicer and page tabs to explore the dashboard.

---

## 👤 Author

**Karan Shinde**
Data Analyst | SQL | Python | Power BI | Tableau | Excel

📧 karanshinde1608@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/karan-shinde-56a35529a)
