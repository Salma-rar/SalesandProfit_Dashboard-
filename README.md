# 📊 Sales & Profit Dashboard

> An end-to-end Business Intelligence project built with **Power BI**, covering data cleaning, data modeling, and interactive dashboard development to analyze sales performance and profitability.

---

## 📁 Repository Structure

```
SalesandProfit_Dashboard/
│
├── 📂 Dashboard/           # Power BI report file (.pbix) with all visuals and KPIs
├── 📂 datamodeling/        # Data model design, relationships, and DAX measures
├── 📂 uncleandData/        # Raw/original data before cleaning and transformation
├── 📄 README.md            # Project documentation
```

---

## 🎯 Project Overview

This project delivers a comprehensive **Sales & Profit Analysis Dashboard** designed to help business stakeholders monitor key performance indicators, identify trends, and make data-driven decisions. The workflow covers the complete BI pipeline — from raw, uncleaned data all the way to a polished, interactive Power BI report.

---

## 🔄 Project Workflow

### 1. 🗃️ Data Collection & Exploration
- Gathered raw sales transactional data stored in the `uncleandData/` folder
- Performed initial exploration to understand the structure, fields, and data quality issues

### 2. 🧹 Data Cleaning & Transformation
- Handled missing values, duplicates, and inconsistent formatting
- Standardized column names, data types, and date formats
- Applied transformations using **Power Query (M Language)** within Power BI

### 3. 🔗 Data Modeling
- Designed a **Star Schema** with fact and dimension tables
- Established relationships between tables (one-to-many)
- Created calculated columns and **DAX measures** for business metrics
- All model artifacts are organized under the `datamodeling/` folder

### 4. 📈 Dashboard Development
- Built an interactive, multi-page Power BI dashboard
- Implemented dynamic filters, slicers, and drill-through pages
- Designed visuals for executive-level reporting

---

## 📌 Key Metrics & KPIs

| KPI | Description |
|-----|-------------|
| **Total Sales** | Aggregate revenue across all products and regions |
| **Total Profit** | Net profit after deducting costs |
| **Profit Margin %** | Profit as a percentage of total sales |
| **Sales Growth** | Period-over-period sales performance |
| **Top Products** | Best-performing products by revenue and profit |
| **Regional Performance** | Sales breakdown by geography |

---

## 📊 Dashboard Features

- **Sales Overview** — High-level KPIs with trend lines and period comparisons
- **Profit Analysis** — Margin tracking by category, region, and time
- **Product Performance** — Ranked view of top/bottom performing products
- **Time Intelligence** — YTD, MTD, and year-over-year comparisons using DAX
- **Interactive Filters** — Slicers for date range, region, category, and segment
- **Drill-Through** — Navigate from summary views into detailed transaction-level data

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Data modeling, DAX, and dashboard development |
| **Power Query (M)** | Data cleaning and transformation |
| **DAX** | Calculated measures and KPIs |
| **Microsoft Excel / CSV** | Source data format |
| **Git & GitHub** | Version control and project hosting |

---

## 💡 DAX Measures (Examples)

```dax
-- Total Sales
Total Sales = SUM(Sales[SalesAmount])

-- Total Profit
Total Profit = SUM(Sales[Profit])

-- Profit Margin %
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)

-- YTD Sales
YTD Sales = TOTALYTD([Total Sales], 'Date'[Date])

-- Sales vs Previous Year
Sales PY = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date]))
```

---

## 🚀 Getting Started

### Prerequisites
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (latest version recommended)

### Steps to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/Salma-rar/SalesandProfit_Dashboard-.git
   ```

2. **Open the report**
   - Navigate to the `Dashboard/` folder
   - Open the `.pbix` file using **Power BI Desktop**

3. **Explore the data model**
   - Go to the **Model View** in Power BI to review table relationships
   - Check the `datamodeling/` folder for documentation on schema design

4. **Interact with the Dashboard**
   - Use slicers and filters to explore different dimensions
   - Use drill-through to navigate to detailed views

---

## 📂 Data Description

| Folder | Contents |
|--------|----------|
| `uncleandData/` | Raw source data files (Excel/CSV) before any processing |
| `datamodeling/` | Schema diagrams, relationship definitions, and DAX documentation |
| `Dashboard/` | Final Power BI `.pbix` file with all pages and visuals |

---

## 🤝 Contributing

Contributions and feedback are welcome!

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m 'Add: your feature description'`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a Pull Request

---

## 👩‍💻 Author

**Salma Rar**
- GitHub: [@Salma-rar](https://github.com/Salma-rar)
- Project Repository: [SalesandProfit_Dashboard](https://github.com/Salma-rar/SalesandProfit_Dashboard-.git)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

*Built with ❤️ using Power BI*
