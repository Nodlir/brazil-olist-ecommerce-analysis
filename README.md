# Brazil-Olist-Ecommerce-Analysis
An end-to-end Power BI project analyzing the Olist Brazilian e-commerce dataset across sales, customer behavior, delivery, payments, and seller performance.

## Dataset

**Source:** https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

Size: 9 relational CSV tables (orders, items, payments, reviews, customers, sellers, products, geolocation, category translation).

Period: 2016 – 2018 | ~99K orders.



## Business Scenario

Olist is a Brazilian marketplace connecting small sellers to customers. Leadership wants one dashboard to monitor business sales and answer questions like:

* **CEO:** "What's our revenue, orders and AOV — and how do they trend?"
* **Marketing Head:** "Who are our best customers, and how many actually come back?"
* **Ops Manager:** "Are we delivering on time, and where are the delays?"
* **CEO:** "Which sellers are underperforming?"



## Objective

* Convert business questions into measurable KPIs and visuals.
* Track **revenue growth** (MoM, YoY, cumulative YTD) and top-performing categories/states.
* Understand **customer retention** using RFM segmentation, repeat-vs-one-time buyers and lifetime value.
* Monitor **delivery performance**, review scores and seller quality.
* Add interactive slicers, parameter toggles and drill-through page for deeper analysis.

## Tools & Skills

| Area | Details |
| :--- | :--- |
| **Tool** | Power BI Desktop |
| **Data prep** | Power Query (cleaning, merging) |
| **Modeling** | Star-schema data model, Fact & Dimension model relationships  |
| **Calculations** | Created DAX measures & calculated columns |
| **Interactivity** | Added Slicers, field parameter toggle, drill-through, tooltips, bookmark buttons |


## Process

1. **Understand requirements** – reviewed stakeholder questions and grouped them into 3 dashboard pages.
2. **Data preparation** – loaded 9 CSVs, cleaning data using Power Query.
3. **Data modeling** – connected fact and dimension tables; created a Date table for time intelligence.
4. **DAX measures** – revenue, orders, AOV, MoM %, YoY %, cumulative YTD, CLV, RFM scores, on-time %, delivery delay, seller rank.
5. **Visual design** – built 3 report pages + 1 drill-through page with consistent theme and KPI cards.
6. **Interactivity** – added year/month slicers, metric-switch parameter, drill-through to detail.
7. **Insights** – Cross-checked key totals and KPI calculations before finalizing the report.



## Key Visualizations (by Objective)

### Page 1 — Sales & Revenue Overview

| # | Stakeholder question | Visual / Measure |
| :--- | :--- | :--- |
| **1** | Total revenue, orders, AOV & monthly trend | KPI cards + Total Revenue by Month (line) |
| **2** | This year vs last year, same period | Total Revenue vs Revenue LY (line) |
| **3** | MoM % and YoY % growth | Growth KPI cards |
| **4** | Running total through the year | Cumulative Revenue YTD (area) |
| **5** | Top 5 categories & % of revenue | Top 5 Revenue Generators (bar, % share) |
| **6** | Toggle Revenue / Orders / AOV | Field parameter + Parameter metrics by Month |
| **7** | Revenue by state vs order volume | Filled map + State breakdown table (orders, revenue per order) |


### Page 2 — Customer Behavior & Retention

| # | Stakeholder question | Visual / Measure |
| :--- | :--- | :--- |
| **8** | RFM segmentation (Champion, At Risk, Lost, New) | RFM Segment Performance table + segment pie |
| **9** | Repeat vs one-time buyers | Customer count by type (pie) |
| **10** | Customer lifetime value | Cust Lifetime Value KPI |
| **11** | New vs returning customers per month | Stacked column by Year & Month |
| **12** | State $\rightarrow$ top customers & order history | Customers by State chart + Top 50 Customers table (drill-through) |

### Page 3 — Delivery, Product & Seller Performance

| # | Stakeholder question | Visual / Measure |
| :--- | :--- | :--- |
| **13** | On-time delivery rate | On-Time Delivery % gauge |
| **14** | Average delay by state / category | Avg Delivery Delay by State & by Product Category (bar) |
| **15** | Review score vs delivery delay | Scatter plot by product category |
| **16** | Seller ranking & bottom 10% | Seller Revenue Ranking & Underperformers table |
| **17** | Payment methods & installments vs order value | Orders by Payment Method + Avg Order Value by Installment Count |
| **18** | Category $\rightarrow$ late orders | Drill-through page: Late Orders — [category] |


## Key Insights

*  **$14M revenue from 99K orders**, with an AOV of $138.
*  **Top 5 categories accounts for 40% of revenue** — health beauty (9.3%), watches gifts (8.9%), bed bath table (7.6%), sports leisure (7.3%), computers accessories (6.7%).
*  **Retention is the biggest gap:** 97% of customers placed only one order, while 3% placed more than one order.
*  **RFM:** 42% of customers are *At Risk* and 30% *Lost*; the few *Champions* spend 4 times more per customer ($584 vs $147).
*  **On-time delivery $\approx$ 92%**: orders typically arrive well before the estimated date.
*  **Late deliveries vs reviews:** Lower review scores are more common among late orders, particularly in some categories. Category-level averages look flat (4 stars), but drilling into late orders (e.g., bed bath table) shows many 1-star ratings.
*  **Credit card is the dominant payment method (75% of orders);** AOV rises sharply with more installments ($120 for 1; $335 for 6+).
*  **Seller revenue is concentrated in Sao Paulo**: the top seller generated $229K in revenue.

## Author

**Rildon Koren** — Data Analyst | Power BI  
🔗 [LinkedIn](https://www.linkedin.com/in/rildon-koren-b11911342/) | ✉️ rildonrk6@gmail.com


  


