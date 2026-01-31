# tableau-sales-analytics

# 📊 Sales Performance & Profitability Dashboard (Tableau)

## Overview
This project presents an interactive Tableau dashboard designed to analyze **sales performance, profitability, and return behavior over time**.  
The goal is to move beyond topline revenue and understand **how margin quality and returns evolve across categories and regions**, enabling more informed business decisions.

The dashboard is built with a **business stakeholder mindset**, emphasizing clarity, comparability, and insight-driven storytelling.

---

## Business Questions
This analysis answers the following key questions:

- How have **sales and profit margins trended over time**?
- Which product categories show **consistent vs volatile profitability**?
- How does **regional sales performance** compare when profitability is considered?
- Are **return rate spikes associated with margin compression**?

---

## Key Metrics
- **Total Sales**
- **Total Profit**
- **Profit Margin (%)**
- **Return Rate (%)**

All metrics are calculated using aggregated values to ensure accurate financial interpretation.

---

## Dashboard Walkthrough & Insights

### 1️⃣ KPI Summary
The dashboard begins with a high-level KPI snapshot:
- Total Sales: **$2.3M**
- Total Profit: **$286K**
- Profit Margin: **12.5%**
- Return Rate: **5.9%**

📌 **Insight:** While overall margins appear healthy, deeper analysis reveals periods of volatility and category-level risk.

---

### 2️⃣ Sales & Profit Trend Over Time
This view separates **sales trends** and **profit margin trends** into two aligned panels:
- Monthly sales trend shown as a time series
- Profit margin plotted independently to avoid misleading dual-axis comparisons
- Reference line highlights the **average profit margin (12.5%)**
- Color encoding emphasizes strong vs weak profitability periods

📌 **Insight:** Sales growth does not always coincide with margin expansion. Several high-revenue periods are associated with below-average profitability, signaling potential discounting or cost pressure.

---

### 3️⃣ Sales by Region
A regional comparison of total sales, colored by profit contribution:
- West and East regions generate the highest revenue
- Central and South lag behind both in sales and profitability

📌 **Insight:** Revenue concentration does not guarantee margin strength, reinforcing the need to evaluate regions through a profitability lens.

---

### 4️⃣ Monthly Sales Trend by Category (Small Multiples)
Small multiple time series for:
- Furniture
- Office Supplies
- Technology

Each category includes:
- Monthly sales trend
- Color encoding by **profit margin**
- A **category-specific average margin reference line**

📌 **Insights:**
- **Technology** exhibits the highest volatility but maintains stronger sustained margins
- **Furniture** shows frequent margin dips despite relatively stable sales
- **Office Supplies** demonstrates steadier performance with fewer extreme swings

This design enables category-level comparison without filtering away context.

---

### 5️⃣ Return Rate Trend
The return rate is visualized as a monthly time series:
- Includes an average return rate benchmark (~6%)
- Highlights sharp spikes across the timeline

📌 **Insight:** Return rate spikes often align with periods of margin compression, suggesting operational or customer experience issues that may impact profitability.

---

## Technical Approach

### Tools
- **Tableau** for visualization and dashboard design

### Calculated Metrics
- **Profit Margin (%)**  
  `SUM(Profit) / SUM(Sales)`
- **Return Rate (%)**  
  Calculated using returned orders relative to total orders

### Tableau Concepts Used
- Horizontal and vertical containers
- KPI tiles with custom alignment
- Small multiples for category comparison
- Reference lines scoped **per pane**
- Diverging color scales centered on meaningful benchmarks
- Custom tooltips for interpretability

---

## Design Principles
- Avoided dual-axis charts to reduce cognitive load
- Used small multiples instead of filters to preserve analytical context
- Centered color scales at zero or average values
- Prioritized business readability over visual density

---

## Repository Structure
