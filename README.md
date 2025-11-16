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

### 1. How is overall transaction performance trending?  
- **Net Sales:** $4.18M  
- **Total Quantity Sold:** 7,534  
- **Average Order Value (AOV):** $562.60  
- Sales peaks occur around **Day 10, Day 15, and Day 24**, indicating predictable high-activity cycles.  
- Revenue spikes result from **high AOV plus elevated order counts**, not just traffic increases.  
- Recovery periods after dips suggest temporary campaign impacts; retention mechanisms underutilized.  
- **Trend Over Time:** synchronized peaks on Day 12, 18, 24; baseline days show potential for micro-campaign uplift.  
- **Insight:** Replicate successful promotional drivers; align acquisition with retention triggers (post-purchase offers, time-limited incentives).

---

### 2. Which customer segments contribute most revenue?  
- **Total Customers:** 4,431  
- **Single-order customers:** 2,392 (54%)  
- **Repeat customers:** 2,039 (46%)  
- Repeat buyers exhibit **higher AOV** and contribute disproportionately to total revenue.  
- Basket-size variance reveals opportunities to segment **high-ticket vs low/mid-ticket customers**.  
- **Insight:** Prioritize converting single-order buyers via **post-purchase flows, cross-sells, and win-back campaigns**; build VIP treatment for high-ticket segments.

---

### 3. What are the dominant product types and payment methods?  
- **Top Product Categories:** Running Shoes, Tennis Shoes, Climbing Shoes, Boots; Flip Flops in select regions.  
- Clear **Pareto distribution**: top product types drive majority of revenue and units sold.  
- Mid-tail SKUs sell steadily but contribute less profit.  
- **Payment Gateways:** Shopify Payments & PayPal dominate volume and revenue; Amazon Pay & Gift Cards smaller but steady.  
- Regional variations in gateway success; some show higher AOV or success in specific metros.  
- **Insight:** Focus merchandising and ad spend on top categories; use bundles to boost mid-tail performance. Optimize checkout UX and monitor top gateways regionally.

---

### 4. How can insights improve retention and customer lifetime value?  
- **Lifetime Value (LTV):** $943.60  
- **Purchase Frequency:** 1.68  
- Repeat customers drive most revenue; single-order buyers represent opportunity for growth.  
- Observed high-ticket, multi-SKU orders indicate natural cross-sell potential.  
- **Insight:** Implement **3-email post-purchase automation** to accelerate time-to-second-purchase, increase LTV, and convert one-time buyers. Build cross-sell bundles and targeted offers for both repeat and high-value segments.

---

### 5. Regional and transactional insights  
- Highest revenue: **California, Texas, Washington, New York, Illinois**  
- Hotspot cities: **Los Angeles, San Diego, San Jose, Dallas, Houston, San Antonio**  
- Smaller markets like **Oklahoma and Florida** have fewer orders but **higher AOV**.  
- **Transactions:** High-ticket orders across gateways/regions; multi-SKU baskets highlight upsell opportunities.  
- **Insight:** Scale volume in CA/TX, deploy premium offers in value-heavy micro-markets, segment flows by basket value, protect top SKUs during peak periods.

---

### 6. Action Plan / Quick Wins  
- Replicate promotional drivers behind **Day 10, 15, 24** via controlled tests.  
- Reallocate ad spend to **top regions/cities** and top 3 metro areas for immediate lift.  
- Develop segmentation clusters:  
  - **Frequency-High Regions** for volume campaigns.  
  - **Value-High Micro-Markets** (e.g., OK, FL) for premium offers.  
- Promote top **20% SKUs** and implement cross-sell bundles to boost attach rate.  
- Strengthen gateway monitoring for Shopify Payments & PayPal and fix region-specific checkout issues.  
- Launch targeted **post-purchase automation** for one-time buyers to accelerate LTV.  
- Protect top 10 highest-value SKUs from stockouts during predicted peak periods.

---

## Technologies & Tools

- **Power BI** – Dashboard development  
- **Excel & Power Query** – Data transformation  
- **DAX** – KPI calculations  


