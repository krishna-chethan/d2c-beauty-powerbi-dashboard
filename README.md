# 📊 D2C Beauty & Personal Care — Impact Reporting Dashboard (Phase 1)

A multi-page, investor-ready Power BI dashboard built for a Direct-to-Consumer (D2C) Beauty and Personal Care brand. This project demonstrates end-to-end BI development — from data modeling and DAX logic to executive-level storytelling across four report pages.

---

## 🗂️ Project Structure

```
d2c-beauty-brand-powerbi/
│
├── README.md
├── krishnachethan-ramadasu_D2C_Phase1.pbix
└── screenshots/
    ├── 01_executive_summary.png
    ├── 02_revenue_performance.png
    ├── 03_cost_margin.png
    └── 04_marketing_attribution.png
```

---

## 📄 Dashboard Pages

### 1. Executive Summary
High-level KPIs for the CEO — revenue, gross margin, units sold, and MoM trends. Designed for a quick pulse check at the board/investor level.

### 2. Revenue & Sales Performance
Breakdown of revenue by product category, channel, and time period. Includes trend analysis with date intelligence (MTD, QTD, YTD comparisons).

### 3. Cost & Margin Analysis
COGS tracking with date-sensitive cost logic — Cost Per Unit varies by time period and is applied accurately using DAX. Gross margin % monitored at SKU and category level.

### 4. Marketing Attribution
Channel-level spend vs. revenue contribution. Helps the CMO identify high-ROI acquisition channels and optimize budget allocation.

---

## 🧱 Data Model

Built on a **Star Schema** architecture:

- **Fact Table:** Sales transactions (order-level granularity)
- **Dimension Tables:** Date, Product, Channel, Customer
- **Key Design Decisions:**
  - Date table built with DAX (`CALENDAR`) for full time intelligence support
  - Cost Per Unit stored in a separate cost table, joined via Product + Date range logic
  - Relationships set to single-direction to avoid ambiguity

---

## 🛠️ Tools & Technologies

| Tool | Usage |
|------|-------|
| Power BI Desktop | Report development, DAX, data modeling |
| Power Query (M) | Data transformation and cleaning |
| DAX | KPI calculations, time intelligence, COGS logic |
| Star Schema | Semantic data model design |

---

## 📁 Data Source

Dataset adapted from the [Goodly Power BI Content Associate Case Study](https://coda.io/d/Power-BI-Content-Associate-Goodly_dKpKGEcnyKm/Case-Study-Phase-1-D2C-Brand-Impact-Reporting_su7dlxKu#_luBsRKPZ) — used for portfolio and practice purposes.

---

## 👤 Author

**Krishna Chethan Ramadasu**
Data Analyst | Power BI Developer
📍 Hyderabad, India
🔗 [LinkedIn](https://www.linkedin.com/in/krishna-chethan-ramadasu-8653521b9/) | 📧 Available on request

---

## 📌 Notes

- This is Phase 1 of the project. Phase 2 will include deeper customer segmentation and cohort analysis.
- The `.pbix` file requires **Power BI Desktop** to open (free download from Microsoft).
- Screenshots are provided for quick preview without needing Power BI installed.
