# Marketing Economics & Contribution Profit Executive Dashboard (Power BI & SQL)

## Project Overview
An end-to-end analytical framework designed to measure customer acquisition efficiency and net profitability across multi-channel campaigns. The project bridges unit economics with marketing performance by tracking Customer Acquisition Cost (CAC), Initial Gross Profit (AGP), and Projected Repeat Gross Profit (RGP) to determine true Contribution Profit.

---

## Visual Preview
![Dashboard Preview](dashboard_overview.png)

---

## Business Value & Core Metrics
* **Contribution Profit:** Evaluates actual bottom-line value after factoring in marketing expenses:  
  $$\text{Contribution Profit} = \text{New Customers} \times (\text{AGP} + \text{RGP} - \text{CAC})$$
* **CAC (Customer Acquisition Cost):** Efficiently scales top-of-funnel ad spend against customer volume:  
  $$\text{CAC} = \frac{\text{Spend}}{\text{New Customers}}$$
* **Initial vs. Repeat Economics:** Incorporates upfront margin (AGP) alongside estimated recurring lifetime profit (RGP).
* **Channel Attribution:** Direct comparative view of ad efficiency across Google Ads, Meta Ads, and TikTok Ads.

---

## Core DAX Formulations

**Customer Acquisition Cost (CAC):**
```dax
CAC = DIVIDE([Total Spend], [Total New Customers], 0)
