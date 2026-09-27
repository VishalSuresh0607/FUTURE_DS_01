# Business Sales Performance Analytics — Power BI

> **One-line summary:** An interactive Power BI dashboard that turns SuperStore sales data into a business view of revenue trends, product/category performance, geographic performance, customer segments, payment modes, delivery, returns, and sales forecasting.

## 🔗 Dashboard & Data Access

| Resource                    | Link                                                                                     |
| --------------------------- | ---------------------------------------------------------------------------------------- |
| **Dataset / Source Data**   | https://docs.google.com/spreadsheets/d/1NI1A7GZfFPKfQmLyYm_xknCTuKGF0fz_/edit?usp=drive_link&ouid=110992777413329417075&rtpof=true&sd=true                                                             |
| **Power BI File (.pbix)**   | [`dashboard/SuperStore_Sales_Dashboard.pbix`](dashboard/SuperStore_Sales_Dashboard.pbix) |

> **Submission note:** The live dashboard and dataset links should be replaced with the actual public/shareable URLs before publishing this repository.

---

## 📸 Dashboard Preview

<img width="1303" height="723" alt="Task1_screenshot" src="https://github.com/user-attachments/assets/0ef66833-e447-4997-9ad0-4a646f55e556" />
_An interactive management view analyzing revenue trends, geographic performance, and key operational metrics._

---

## 1. Business Problem

Businesses need a quick way to understand **where revenue is coming from, how sales change over time, which products and categories drive performance, and which regions require attention**.

The purpose of this dashboard is to answer:

- How is sales performance changing over time?
- Which categories and sub-categories contribute the most sales?
- Which states/regions generate the strongest sales?
- How are sales distributed across customer segments and payment modes?
- What do quantity, returns, delivery performance, and profitability indicate about the overall business?
- What does the historical sales trend suggest for future planning?

The dashboard converts these questions into an interactive management view so a stakeholder can move from a high-level KPI view to category, product, geographic, and time-based analysis.

---

## 2. Key Insights

The current report is structured to surface the following business insights:

1. **Revenue / Sales Trend** — Monthly sales performance can be examined over time to identify growth patterns, fluctuations, and periods requiring further investigation.
2. **Category & Sub-category Performance** — Sales are broken down by category and sub-category, making it possible to identify the major revenue contributors and weaker product groups.
3. **Geographic Performance** — State-level sales are visualized geographically and through a ranked bar chart, helping identify high-value and lower-performing locations.
4. **Customer & Payment Mix** — Sales are segmented by customer segment and payment mode to understand how different customer groups and transaction methods contribute to revenue.
5. **Operational Indicators** — Quantity, returns, average delivery performance, profit, and historical/forecast sales views provide additional context beyond revenue alone.

### Important reporting discipline

Exact numerical rankings, percentages, and values should be copied from the final dashboard before publication. This repository intentionally avoids inventing figures that are not independently extracted from the report.

---

## 3. Tools & Technologies

- **Microsoft Power BI** — dashboard development, data modeling, interactive visual analytics
- **Power BI data model / DAX measures** — KPI and analytical calculations where applicable
- **SuperStore sales dataset** — primary analytical data source
- **GitHub** — versioning, documentation, and project presentation
- **Power BI Service** — recommended platform for publishing the live interactive report

### Metrics represented in the report

The report includes analysis around:

- Sales
- Profit
- Quantity
- Returns
- Average Delivery
- Order Date
- Category
- Sub-category
- State
- Region
- Segment
- Payment Mode
- Ship Mode

---

## 4. Dashboard Pages & Navigation

### Page 1 — Sales Performance Dashboard

The primary dashboard provides a management-level overview. It includes:

- Total Sales KPI
- Total Quantity KPI
- Returns KPI
- Average Delivery KPI
- Region filter
- Sales by Category
- Sales by Sub-category
- Sales by State
- Sales trend over time
- Profit trend over time
- Sales by Customer Segment
- Sales by Payment Mode
- Sales by Ship Mode

**Recommended stakeholder workflow:**

1. Start with the KPI cards to understand the overall business position.
2. Use the **Region** slicer to isolate a geographic area.
3. Check the **sales trend** to understand time-based movement.
4. Move to **Category / Sub-category** charts to identify product-group contribution.
5. Review the **state map and state ranking** to locate strong and weak markets.
6. Use **segment, payment mode, and ship mode** views to understand customer and operational mix.
7. Compare sales with **profit, returns, quantity, and delivery indicators** before making a business interpretation.

### Page 2 — Sales Forecast

The report also contains a dedicated **SuperStore Sales Forecast** page with historical/forecast sales trend visuals and a state-level sales view.

This page can support planning discussions, but forecast outputs should be treated as analytical estimates rather than guaranteed future results.

---

## 5. Methodology

The analysis follows a typical business intelligence workflow:

**Source Data → Data Preparation → Data Model → Measures/KPIs → Visual Analysis → Business Interpretation**

### Data preparation

The source SuperStore dataset is used as the analytical foundation. The report organizes fields such as dates, geography, product hierarchy, customer segment, sales, profit, quantity, returns, and delivery information for interactive analysis.

### Analysis approach

- Aggregate sales and quantity for KPI reporting.
- Analyze sales and profit across time.
- Compare category and sub-category performance.
- Examine state/region-level sales.
- Segment sales by customer and payment characteristics.
- Include operational indicators such as returns and delivery.
- Use historical sales patterns as the basis for the forecast page.

### Data quality note

Before using the dashboard for an actual business decision, validate the source dataset, date range, currency, missing values, duplicate records, return definitions, and forecast assumptions against the organization's source systems.

---

## 6. Repository Structure

```text
power-bi-business-sales-performance-analytics/
│
├── dashboard/
│   ├── SuperStore_Sales_Dashboard.pbix
│   └── README.md
│
├── data/
│   └── README.md
│
├── documentation/
│   ├── INSIGHTS.md
│   └── METHODOLOGY.md
│
├── README.md
└── .gitignore
```

### File guide

- **`dashboard/`** — Power BI report and dashboard access notes.
- **`data/`** — source dataset or instructions/link to the dataset.
- **`documentation/`** — supporting insight and methodology documentation.
- **`README.md`** — project overview and stakeholder guide.

---

## 7. How a Business Stakeholder Can Use This

A business owner, startup founder, sales manager, or analytics client can use the dashboard to:

- Monitor overall sales performance.
- Identify major revenue-generating product groups.
- Compare geographic markets.
- Investigate changes in sales over time.
- Understand customer and transaction mix.
- Compare sales with profit and operational indicators.
- Use the forecast page as an input for planning conversations.
- Drill into areas that require additional investigation.

The dashboard is designed to **support business questions rather than simply display charts**.

---

## 8. Business Value

The key value of this project is the conversion of a raw sales dataset into a **decision-oriented analytical interface**.

Instead of requiring a stakeholder to manually inspect rows of transactional data, the dashboard provides a single place to explore:

**Performance → Trend → Product → Geography → Customer → Operations → Forecast**

This structure makes the analysis easier to communicate and gives stakeholders a practical starting point for deeper business investigation.

---

## 9. Limitations

- The dashboard reflects the quality and scope of the underlying dataset.
- Historical sales patterns do not guarantee future performance.
- Forecast outputs should be interpreted together with business context.
- Sales alone should not be treated as the complete measure of business health; profit, returns, costs, delivery performance, and customer behavior should also be considered.
- Any client deployment should use validated business definitions and current source-system data.

---

## 10. Internship Context

**Task 1 of 3 — Business Sales Performance Analytics**

This project demonstrates practical experience in:

- Business problem framing
- Power BI dashboard development
- KPI design
- Exploratory data analysis
- Business-oriented visualization
- Geographic and product performance analysis
- Forecast-oriented reporting
- Technical documentation

The objective is to present the work as a **client-ready analytics project**, not simply as a classroom dashboard.

---

## 11. Author

**Vishal Suresh**  
Electrical and Computer Engineering Student  
Interested in Data Analytics, AI, Machine Learning, and Technology

---

## License / Usage

If the underlying SuperStore dataset belongs to a third party, retain its original attribution and usage terms. The Power BI report in this repository is provided for portfolio and educational/internship demonstration purposes unless otherwise stated.
