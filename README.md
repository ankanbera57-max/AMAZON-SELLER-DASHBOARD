# 📊 Amazon Seller Sales & Performance Analytics

An interactive Power BI analytics dashboard analyzing **$7.49M** in e-commerce sales, **2,000+** customer orders, and **$1.15M** net profit (**15.33%** operating margin) across regional markets and fulfillment channels.

---

## 📌 Dashboard Overview

![Amazon Dashboard](AMAZON%20SELLER%20DASHBOARD%20.png)

---

## 🏢 Business Problem & Objectives
This project provides actionable operational visibility for Amazon sellers by addressing:
1. **Channel & Regional Efficiency:** Identifying which fulfillment channels and geographic regions generate highest order volume vs. margins.
2. **Product Profitability:** Segmenting high-margin SKUs from low-velocity items to streamline inventory.
3. **Marketing Budget Optimization:** Analyzing advertising spend against realized net profits to curb capital leakage on low-return products.

---

## 🔑 Key Performance Indicators (KPIs)
* **Total Revenue:** $7.49M across regional fulfillment centers
* **Order Volume:** 2,000+ orders processed
* **Net Profit:** $1.15M net realized profit
* **Operating Profit Margin:** 15.33%

---

## 💡 Strategic Business Insights
* **Top Profit Contributor:** Mechanical Keyboards and Smart Watches generated the highest aggregate net profit, validating strong organic demand.
* **Ad Spend vs. Profitability:** Marketing expenditure on lower-tier electronics accessories exhibited diminishing returns; shifting 15% of that budget toward top-margin SKUs can boost overall margin by ~2.4%.
* **Fulfillment Distribution:** North and South fulfillment regions account for over 50% of aggregate volume, indicating opportunities for regional stock prioritization.

---

## 🛠️ Technical Stack & Implementation
* **Tool:** Microsoft Power BI Desktop
* **Data Modeling:** Star Schema architecture, custom KPI cards, and regional distribution bar charts
* **Key DAX Measure:**
  ```dax
  Profit Margin = 
  DIVIDE(
      SUM('Amazon Sales Data'[Profit]),
      SUM('Amazon Sales Data'[Sales])
  )
