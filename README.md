<h1 align="center">📊 Power BI Sales Analytics Dashboard</h1>

<p align="center">
  <b>A single-page executive view of sales, profit, customers, products, channels and regions.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI"/>
  <img src="https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white" alt="DAX"/>
  <img src="https://img.shields.io/badge/Power_Query-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="Power Query"/>
  <img src="https://img.shields.io/badge/Star_Schema-5C2D91?style=for-the-badge" alt="Star Schema"/>
</p>

<p align="center">
  <a href="#-dashboard-preview">Preview</a> •
  <a href="#-key-features">Features</a> •
  <a href="#-key-insights">Insights</a> •
  <a href="#-dax-measures">DAX</a> •
  <a href="#-getting-started">Getting Started</a>
</p>

---

## 📖 Overview

This interactive Power BI report monitors **sales performance and business trends** in one place. It combines KPI cards with year-over-year comparisons, monthly trends, category, channel and regional analysis, salesperson and product performance, and a short management insights panel.

**Reporting period:** 2024
---

## 📊 Headline Numbers

| Metric | Value | vs Last Year |
|---|:---:|:---:|
| 💰 **Total Sales** | $55.9M | 🟢 +18.15% |
| 📈 **Total Profit** | $5.5M | 🟢 +31.90% |
| 🛒 **Total Orders** | 348,125 | 🟢 +15.87% |
| 👥 **Total Customers** | 18,765 | 🟢 +15.58% |
| 🧾 **Avg Order Value** | $160.55 | 🟢 +2.03% |
| 🎯 **Profit Margin** | 9.83% | 🟢 +0.95 pp |

---

## ✨ Key Features

| | Feature | Description |
|:---:|---|---|
| 🧮 | **KPI Cards** | Sales, profit, orders, customers, AOV and margin with last-year comparison |
| 📅 | **Monthly Trend** | Combined column and line chart of sales and profit by month |
| 🍩 | **Sales by Category** | Donut chart of category contribution |
| 🌍 | **Sales by Region** | Bar chart comparing countries |
| 🛍️ | **Sales by Channel** | Online, Retail Store, Distributor and Others |
| 🧑‍💼 | **Top 6 Sales Persons** | Sales, orders, profit and margin % |
| 🏷️ | **Top 10 Products** | Sales, profit and margin % with conditional formatting |
| 💡 | **Key Insights Panel** | Short management summary of the main findings |
| 🔗 | **Interactive Filtering** | Click any visual to filter the rest of the report |

---

## 🎯 Business Objectives

- Monitor total sales, profit, orders, customers, AOV and profit margin
- Compare current performance with the previous year
- Identify monthly sales and profit trends
- Understand which categories and channels drive revenue
- Compare sales across countries
- Track individual salesperson performance
- Identify high-performing, profitable products

---

## 🔍 Key Insights

### 🏆 Top Performers

| Category | Leader | Value |
|---|---|---|
| Category | Consumer Goods | $18.2M (32.5%) |
| Channel | Online | $30.2M (54.0%) |
| Region | USA | $20.9M |
| Salesperson | Aarav Sharma | $8.7M sales, 6.67% margin |
| Product (sales & profit) | Chocolate Wafer Pack | $3.4M sales, $1.02M profit |
| Product (margin) | Hydration Electrolyte | 32.86% |

### 🍩 Sales by Category

| Category | Sales | Share |
|---|---:|---:|
| Consumer Goods | $18.2M | 32.5% |
| Food & Beverages | $13.7M | 24.5% |
| Home Appliances | $9.6M | 17.2% |
| Personal Care | $7.1M | 12.7% |
| Sports & Fitness | $4.6M | 8.2% |
| Others | $2.7M | 4.9% |

### 🛍️ Sales by Channel

| Channel | Sales | Share |
|---|---:|---:|
| Online | $30.2M | 54.0% |
| Retail Store | $15.7M | 28.1% |
| Distributor | $7.4M | 13.2% |
| Others | $2.6M | 4.7% |

### 🌍 Sales by Region

| Region | Sales |
|---|---:|
| USA | $20.9M |
| UK | $10.2M |
| Canada | $7.4M |
| Australia | $5.4M |
| India | $5.0M |
| New Zealand | $3.0M |
| Others | $3.8M |

### 🧑‍💼 Top 6 Sales Persons

| Sales Person | Sales | Orders | Profit | Margin |
|---|---:|---:|---:|---:|
| Aarav Sharma | $8.7M | 52,340 | $0.58M | 6.67% |
| Neha Verma | $8.1M | 48,266 | $0.52M | 6.42% |
| Rohit Mehta | $7.9M | 51,008 | $0.50M | 6.33% |
| Priya Nair | $7.5M | 46,712 | $0.47M | 6.22% |
| Vikram Rao | $7.1M | 44,896 | $0.44M | 6.19% |
| Sneha Iyer | $6.6M | 41,903 | $0.41M | 6.07% |

### 🏷️ Top 10 Products

| Product | Sales | Profit | Margin |
|---|---:|---:|---:|
| Chocolate Wafer Pack | $3.4M | $1.02M | 30.00% |
| Vanilla Protein Bar | $3.1M | $0.98M | 31.61% |
| Energy Drink (250ml) | $2.9M | $0.86M | 29.66% |
| Oats & Honey Cereal | $2.7M | $0.82M | 30.37% |
| Green Tea (50g) | $2.5M | $0.78M | 31.20% |
| Almond Face Wash | $2.3M | $0.72M | 31.30% |
| Hydration Electrolyte | $2.1M | $0.69M | 32.86% |
| Multigrain Biscuits | $2.0M | $0.63M | 31.50% |
| Body Lotion (200ml) | $1.9M | $0.58M | 30.53% |
| Smart LED Bulb | $1.8M | $0.55M | 30.56% |

---

## 📐 DAX Measures

```dax
-- Core measures
Total Sales     = SUM(Sales[Sales Amount])
Total Profit    = SUM(Sales[Profit])
Total Orders    = DISTINCTCOUNT(Sales[Order ID])
Total Customers = DISTINCTCOUNT(Sales[Customer ID])

-- Ratios
Average Order Value = DIVIDE([Total Sales], [Total Orders])
Profit Margin %     = DIVIDE([Total Profit], [Total Sales])

-- Time intelligence
Sales LY  = CALCULATE([Total Sales],  SAMEPERIODLASTYEAR('Dim Date'[Date]))
Profit LY = CALCULATE([Total Profit], SAMEPERIODLASTYEAR('Dim Date'[Date]))

Sales Growth % = DIVIDE([Total Sales] - [Sales LY], [Sales LY])
```

> **Note:** Table and column names should match your own data model. `SAMEPERIODLASTYEAR` requires a properly related, continuous date table.

---

## 🧱 Data Model

A **star schema** with a central Sales fact table and supporting dimensions:

| Table | Typical Columns |
|---|---|
| **Fact Sales** | Order ID, Date Key, Product Key, Customer Key, Salesperson Key, Channel Key, Region Key, Quantity, Sales Amount, Cost, Profit |
| **Dim Date** | Date, Month, Month Number, Quarter, Year |
| **Dim Product** | Product ID, Product Name, Category, Subcategory |
| **Dim Customer** | Customer ID, Customer Name, Country/Region |
| **Dim Salesperson** | Salesperson ID, Name, Team/Region |
| **Dim Channel** | Channel ID, Channel Name |
| **Dim Region** | Region/Country, Territory |

---

## 🛠️ Skills Demonstrated

- 🔧 Data import and transformation with Power Query
- 🧱 Data modeling and relationships
- 📅 Date-table design and time intelligence
- 🧠 DAX measures and KPI calculations
- 📊 KPI cards, column, line, donut and bar charts, and tables
- 🎨 Conditional formatting and dashboard storytelling
- 🔗 Interactive filtering

---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git

# Move into the project folder
cd YOUR-REPO
```

1. Open the `.pbix` file in **Power BI Desktop**
2. Go to **Home → Transform data → Data source settings** and point to your local data files
3. Click **Refresh**

---

## 📁 Repository Structure

```text
├── assets/
│   └── dashboard.jpeg
├── docs/
│   └── Power_BI_Sales_Analytics_Project_Documentation.pdf
├── data/
├── Sales_Analytics_Dashboard.pbix
└── README.md
```

---

## 📝 Conclusion

This dashboard gives a consolidated view of sales and profitability, and works as a portfolio project for demonstrating data modeling, DAX, visualization, KPI reporting and business-oriented analysis.

---

<p align="center">⭐ If you found this project useful, give it a star!</p>
