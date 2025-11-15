# Shopify Customer & Sales Analytics

Real-time, applied analytics on Shopify transactions and customer behavior using Power BI dashboards. This project provides actionable insights into sales performance, customer engagement, and retention trends to support data-driven decision-making.

<img width="848" height="502" alt="Shopify Analysis Dashboard" src="https://github.com/user-attachments/assets/6ee532d0-a448-492b-be3e-8bad94f81bd3" />

---

## Project Overview

The goal of this project is to analyze Shopify sales data in Power BI to uncover meaningful insights into transaction performance, customer purchasing behavior, and long-term customer value.

By designing interactive dashboards, the project enables stakeholders to:
- Track revenue generation and sales trends over time  
- Understand customer behavior, including single vs repeat purchase patterns  
- Evaluate customer retention and lifetime value (LTV) metrics  
- Make informed decisions for business strategy and marketing campaigns  

---

## Dataset

The dataset is derived from Shopify transactional records and contains detailed sales and customer information.

| Column Name | Description |
|-------------|-------------|
| Admin GraphQL API ID | Unique identifier used by backend systems |
| Order Number | Unique order ID |
| Billing Address City | Customer’s billing city |
| Billing Address Country | Customer’s billing country |
| Billing Address First/Last Name | Customer details |
| Billing Address Province | Province/state for reporting |
| Billing Address Zip | Postal code |
| CITY | City field variant |
| Currency | ISO currency |
| Customer ID | Unique customer identifier |
| Invoice Date | Transaction date |
| Gateway | Payment method |
| Product ID | Unique product identifier |
| Product Type | Category of product |
| Variant ID | Product variant |
| Quantity | Units purchased |
| Subtotal Price | Price before tax |
| Total Price USD | Final price in USD |
| Total Tax | Tax applied |

---

## Problem Statement

This analysis answers critical business questions:

1. How is overall transaction performance trending?
2. Which customer segments contribute most revenue?
3. What are the dominant product types and payment methods?
4. How can insights improve retention and customer lifetime value?

---

## Key Performance Indicators (KPIs)

### Transaction Performance
| KPI | Definition |
|------|-----------|
| Net Sales | Total revenue before tax |
| Total Quantity | Total units sold |
| Net Avg Order Value | Average revenue per order |

### Customer Purchase Behavior
| KPI | Definition |
|------|-----------|
| Total Customers | Unique buyers |
| Single Order Customers | One-time buyers |
| Repeat Customers | Buyers with multiple purchases |

### Retention & Value KPIs
| KPI | Definition |
|------|-----------|
| Lifetime Value (LTV) | Total revenue per customer |
| Repeat Rate | % of customers returning |
| Purchase Frequency | Average orders per customer |

---

## Methodology

1. **Data Collection** – Extracted Shopify order, customer, product, and gateway data.  
2. **Data Cleaning** – Standardized fields, removed duplicates, unified currency.  
3. **EDA** – Identified key sales, product, and customer patterns.  
4. **KPI Calculation** – Built DAX measures for performance, retention, and value metrics.  
5. **Dashboard Design** – Created overview, drill-through, customer, and regional dashboards.  
6. **Insights & Recommendations** – Interpreted trends for revenue, retention, and product performance.


---

## Dashboards

### Overview Dashboard
<img width="848" height="502" alt="Shopify Analysis Dashboard" src="https://github.com/user-attachments/assets/78031fb4-83ac-4916-8618-004fd8be848f" />

### Details Dashboard
<img width="848" height="499" alt="Details Dashboard" src="https://github.com/user-attachments/assets/233beecc-bd9c-41b7-bccd-99d6b78ba52b" />

### Filtered Total Customers Dashboard – deeper customer segmentation.  

<img width="849" height="500" alt="Total Customers Dashboard" src="https://github.com/user-attachments/assets/d5087236-de83-466e-aed8-77fd338e321e" />


### Filtered California Province Dashboard – geographic insights for California.

<img width="848" height="499" alt="Califonia State" src="https://github.com/user-attachments/assets/032df2d0-8f99-4192-9c85-df04a2a345f9" />


---

## Results & Insights

## Key Metrics
- **Net Sales:** $4.18M  
- **Total Quantity Sold:** 7,534  
- **Average Order Value (AOV):** $562.60  
- **Insight:** Strong AOV combined with periodic order surges indicates highly effective promotional windows that can be replicated and optimized further.

---

## Transaction Performance
- Sales peaks occur consistently around **Day 10, Day 15, and Day 24**, indicating clear high-activity cycles.
- Revenue surges are driven by a combination of **higher AOV** and **elevated order volume**, not just increased site traffic.
- Baseline days show significantly lower activity, signaling potential to elevate everyday performance with micro-campaigns.
- **Insight:** Mirror successful promotional drivers from peak days. Test bundling, upsells, and micro-offers on baseline days to lift daily revenue.

---

## Trend Over Time
- Sales and customer activity trend together, with synchronized peaks on **Day 12, Day 18, and Day 24**.
- Each peak is followed by a noticeable dip, indicating campaign impacts are strong but short-lived.
- Recovery suggests that while activation works, **retention mechanisms are currently underutilized**.
- **Insight:** Align acquisition bursts with immediate retention triggers—post-purchase offers, rapid re-engagement, and time-limited incentives.

---

## Regional Performance
- Highest revenue comes from **California, Texas, Washington, New York, and Illinois**.
- Strong performing cities include **Los Angeles, San Diego, San Jose, Dallas, Houston, and San Antonio**.
- Smaller markets like **Oklahoma and Florida** deliver fewer orders but exhibit **higher AOV**, forming value-heavy micro-markets.
- **Insight:**  
  - Scale volume and acquisition efforts in CA & TX.  
  - Apply VIP and premium pricing/upsell strategies in high-AOV micro-markets.

---

## Product Performance
- Dominant revenue categories: **Running Shoes, Tennis Shoes, Climbing Shoes, and Boots**.
- Select regions show high turnover for **Flip Flops**, suggesting seasonal or demographic-driven spikes.
- A classic **Pareto distribution** exists — top product types generate the majority of revenue.
- Mid-tail products sell steadily but contribute less to profit.
- **Insight:** Maximize spend and visibility on top categories. Use bundles and cross-category promotions to elevate mid-tail products without hurting bestsellers.

---

## Payment Gateway Behavior
- **Shopify Payments** and **PayPal** dominate both transaction volume and total revenue.
- **Amazon Pay** and **Gift Cards** show steady but smaller contribution.
- Gateway effectiveness varies slightly by metro — certain regions show higher AOV or better checkout success with specific gateways.
- **Insight:** Strengthen UX, reduce friction, and enhance monitoring for Shopify Payments & PayPal. Investigate and fix region-specific gateway decline points.

---

## Customer Behavior & Retention
- **Total Customers:** 4,431  
- **Single-order customers:** 2,392 (54%)  
- **Repeat customers:** 2,039 (46%)  
- **Lifetime Value (LTV):** $943.60  
- **Purchase Frequency:** 1.68  
- Repeat buyers show **higher AOV** and contribute disproportionately to total revenue.
- **Insight:** Deploy targeted retention strategies to convert single-order customers—post-purchase sequences, time-limited cross-sells, and win-back flows.

---

## Transaction-Level Observations
- Top transactions include frequent high-ticket orders across multiple gateways and regions.
- Wide variance in basket sizes reveals strong segmentation opportunities by purchase value.
- Many large orders contain multiple items from top categories, highlighting **strong natural cross-sell behavior**.
- **Insight:** Build a “high-ticket” segment for enhanced VIP experience and dedicated upsell pathways; design separate flows for low- and mid-ticket customers.

---

## Action Plan  
- Identify the specific promotional factors behind peak days (**Day 10, Day 15, Day 24**) and replicate through controlled experiments.
- Shift ad spend toward top-performing regions and cities (especially **CA & TX**, plus Los Angeles, San Diego, Dallas, Houston).
- Develop segmentation clusters:
  - **Frequency-High Regions** for scaling volume.
  - **Value-High Micro-Markets** (e.g., OK, FL) for premium offers.
- Promote the top **20% SKUs** aggressively and build cross-sell bundles to boost attach rate.
- Strengthen gateway monitoring for Shopify Payments & PayPal and fix region-dependent checkout failures.
- Launch a **3-email post-purchase automation** to convert single-order buyers and accelerate time-to-second-purchase.
- Reallocate a portion of ad spend to top 3 metro areas for faster acquisition gains.
- Protect top 10 highest-value SKUs from out-of-stock risk during predicted peak periods.

---

## Technologies & Tools

- **Power BI** – Dashboard development  
- **Excel & Power Query** – Data transformation  
- **DAX** – KPI calculations  

---


