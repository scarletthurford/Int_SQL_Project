 # Intermediate SQL - Sales Analysis

 ## Overview

 Analysis of customer behaviour, retention, and lifetime value for an e-commerce company to improve customer retnetion and maximise revenue.

 ### Tools 
- **Database:** PostgreSQL
- **Analysis Tools:** PostgreSQL in DBeaver

 ## Business Questions

 1. **Customer Segmentation:**
 2. **Cohort Analysis:** How do different customer groups generate revenue?
 3. **Customer Retention:** 

## Analysis Approach

### 1. Customer Segementation Analysis

- Categorised customers based on total lifetime value (LTV)
- Assigned customers to High, Mid, and Low-value segments
- Calculated total revenue

Query: [1_customer_segmentation.sql](1_customer_segmentation.sql)

**Key Findings:**

- High-value segment (25% of customers) drives 66% of revenue
- Mid-value segment (50% of customers) generates 32% of revenue 
- Low-value segment only drives 2% of revenue

**Business Insights**

- Mid-Value: Created upgrade paths through personalised promotions
- Low-Value: Design re-engagement campaigns and price-sensitive promotions to increase purchase frequency

### 2. Cohort Analysis 

- Tracked revenue and customer count per cohorts
- Cohorts were groups by year of first purchase
- Analysed customer retention at a cohort level

Query: [2_cohort_analysis.sql](/2_cohort_analysis.sql)

**Key Findings:**

- Revennue per customer is decreasing over time.
- 2022-2024 cohorts are consistently perorming worse than earlier cohorts.
- Although net revenue is increasing, this is likely due to a larger customer base, which is not reflective of customer value.

**Business Insights**
- Value extraced from customers is decreasing over time.
- In 2023, there was a drop in customers acquired.
- With both lowering LTV and decreasing customer acquisition, the company is facing a potential revenue decline.

### 3. Customer Retention

- Identified customers at risk of churning
- Analysed last purchase patterns
- Calculated customer-specific metrics

Query: [3_retention_analysis.sql](/3_retention_analysis.sql)

**Key Findings:**
 
 - Cohort churn stabilises at ~90% after 2-3 years, indicating a predicatable long-term retention pattern.
 - Retention rates are consistently low (8-10%) across all cohorts, suggesting retention issues are systemic rather than specific to certain years.
 - Newer cohorts (2022-2023) show similar churn trajectories, suggesting that future cohorts will follow the same pattern if there are no efforts to intervene.

 **Business Insights**

 - Strengthen early engagement strategies to target the first 1-2 years with onboarding incentives, loyalty rewards, and personalised offers to improve long-term retention.
 - Re-engaged high-value churned customers by focusing on targeted win-back campaigns rather than broad retention efforts, as reactivating valuable users may yield higher ROI.
