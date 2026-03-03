# Customer Lifetime Value (CLV) & RFM Segmentation – E-Commerce Analytics

## Project Overview

This project delivers an end-to-end customer analytics system designed to identify high-value customers, quantify lifetime profitability, detect churn risk, and optimize marketing capital allocation.

The objective was to transition from revenue-based reporting to margin-driven, customer-level decision intelligence using SQL, Excel, and Power BI.

---

## Business Problem

The organization lacked a structured framework to:

- Identify economically valuable customers  
- Allocate marketing budget efficiently  
- Measure lifetime profitability  
- Detect churn risk proactively  
- Optimize discount and retention strategies  

Marketing investment decisions were driven primarily by revenue volume rather than margin contribution or lifetime value.

---

## Solution Architecture

The system was built across three analytical layers:

### 1. MySQL – Historical Truth Layer
- 3NF normalized schema design  
- Transaction-level validation and integrity checks  
- Customer 360 aggregation  
- Percentile-based RFM segmentation (NTILE)  
- Margin-adjusted CLV modeling  
- Recency-based churn classification  
- Channel and category profitability analysis  

### 2. Excel – Financial Simulation Layer
- CLV elasticity modeling  
- Retention improvement scenarios  
- Frequency uplift simulation  
- Discount sensitivity analysis  
- Segment-level ROI estimation  
- Capital allocation modeling  

### 3. Power BI – Executive Decision Layer
- Star schema modeling  
- DAX-based KPI calculations  
- Interactive executive dashboard (multi-page)  
- Segment, channel, and region-level slicing  
- Profitability and churn visualization  

---

## Analytical Methodology

### RFM Segmentation

Customers were ranked using percentile-based scoring:

- **Recency** – Time since last purchase  
- **Frequency** – Number of completed orders  
- **Monetary** – Revenue contribution  

This ensured segmentation was statistically scaled and dataset-independent.

---

### CLV Modeling

**Revenue CLV**

CLV = (AOV × Frequency) / Churn Rate

**Margin CLV (Profit-Based)**

CLV = (AOV × Frequency × Margin %) / Churn Rate

This approach ensures customer value reflects profitability rather than gross revenue.

---

### Churn Definition

Churn was defined as:

Recency > 180 days

Segment-wise churn analysis was used to detect revenue leakage concentration.

---

## Key Insights

- Customer value is highly concentrated in top-tier segments.
- Retention improvement delivers significantly higher CLV uplift than discount-based growth.
- Certain acquisition channels generate high revenue but lower margin per customer.
- Mid-tier customers represent the largest scalable retention opportunity.
- Blanket discounting erodes long-term profitability.

---

## Financial Simulation Findings

Scenario modeling revealed:

- A 5% retention improvement generates disproportionately higher CLV growth than a 10% frequency increase.
- Discount reduction improves margin CLV but must be segment-targeted.
- ROI varies significantly across segments — not all customers justify retention investment.

**Conclusion:**  
Retention-driven growth is more capital-efficient than acquisition-heavy expansion.

---

## Strategic Recommendations

### Retention Strategy
- Prioritize high and mid-value segments for retention investment.
- Implement recency-based churn monitoring.
- Avoid excessive discounting for high-value customers.

### Acquisition Strategy
- Reallocate budget toward high-margin acquisition channels.
- Reduce spend on low CLV-generating channels.
- Expand referral-based sourcing.

### Pricing Strategy
- Replace blanket discounts with targeted loyalty incentives.
- Protect high-margin categories from aggressive discount exposure.

---

## Business Impact

This project transforms transactional data into:

- Customer-level profitability intelligence  
- Segment-based capital allocation decisions  
- Churn risk visibility  
- Margin-optimized marketing strategy  

The result is a scalable, data-driven framework for revenue growth and profitability optimization.

---

## Tools & Technologies

- MySQL (Data Modeling & KPI Engineering)  
- Excel (Financial Simulation & Scenario Analysis)  
- Power BI (Executive Dashboard & DAX Modeling)  

---

## Conclusion

This project demonstrates a complete analytics lifecycle:

- Data validation  
- Customer segmentation  
- Lifetime value modeling  
- Financial simulation  
- Executive visualization  
- Strategic recommendation  

It reflects production-grade business analytics thinking focused on profitability, retention, and capital efficiency.
