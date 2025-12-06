# **Customer RFM Segmentation Project**
![SQL](https://img.shields.io/badge/SQL-MySQL-orange) →![Python](https://img.shields.io/badge/Python-3.10%2B-blue)→![Power BI](https://img.shields.io/badge/BI-Power%20BI-yellow)

**Project Overview**
This project performs end-to-end customer segmentation using the RFM (Recency, Frequency, Monetary) framework combined with Customer Lifetime Value (CLV) analytics.
The objective is to identify high-value customers, loyal buyers, potential growth segments, at-risk customers, and churned customers.

This is a complete SQL → Python → SQL → Python → Power BI analytics pipeline, similar to real-world workflows used in e-commerce and retail companies.

<img src="https://raw.githubusercontent.com/priyankadatacodes/customer-rfm-analysis/main/workflowdiagram.png" width="100%">


---

## **Business Problem**

The business was treating all customers uniformly without knowing:
- Which customers generate the most revenue
- Who buys frequently vs. occasionally
- Which customers are at risk of churn
- Which segments justify higher marketing investment

This led to inefficient marketing spend, poor retention, and revenue loss.

---

## **Project Objective**

- Implement RFM analysis on customer transactional data  
- Assign NTILE-based scores to Recency, Frequency, and Monetary metrics  
- Classify customers into strategic behavioral groups  
- Enrich RFM output with CLV and retention indicators  
- Deliver final dataset for BI dashboard insights and decisions  

---

## **End-to-End Workflow**

**Dataset Link:** https://www.kaggle.com/datasets/rajneesh231/retail-insights-a-comprehensive-sales-dataset


SQL → Python → SQL → Python → Power BI

1. SQL — Raw Table Setup
Create transactional tables
Validate raw data format
Prepare data for preprocessing

2. Python — Data Cleaning and Export
Remove duplicates
Handle missing values
Fix date formats
Export cleaned data back into SQL

3. SQL — RFM Calculation and Segmentation
Calculate Recency, Frequency, Monetary metrics
Assign quantile-based scores (1–5)
Create customer segments

4. Python — CLV Modeling and Final Dataset Creation
Import RFM output
Compute Customer Lifetime Value
Merge and enrich customer segmentation dataset
Export final dataset for BI

5. Power BI — Dashboard Development
Build RFM dashboard
Create CLV comparison visuals
Add insight-based KPIs and segment summaries

**Dataset Link:** https://www.kaggle.com/datasets/rajneesh231/retail-insights-a-comprehensive-sales-dataset

## **Dashboard**

<img src="https://raw.githubusercontent.com/priyankadatacodes/customer-rfm-analysis/main/dashboard/rfm_analysis_dashboard.png" width="100%">

This interactive Power BI dashboard provides a complete view of customer behavior using Recency, Frequency, Monetary (RFM) segmentation combined with Customer Lifetime Value (CLV) insights.
It helps identify high-value customers, loyal segments, potential growth groups, and customers at churn risk.

## **Key Insights Delivered**

1. Customer segments behave very differently
Champions and Loyal customers generate most revenue
Lost customers form a large portion but contribute very little
Potential customers show high future value

2. Recency trends indicate retention challenges
Many customers have not purchased recently
At-risk customers require immediate attention

3. Frequency reveals loyalty patterns
Loyal customers buy more frequently
Lost customers show minimal repeat behavior

4. Monetary and CLV highlight profitability
Potential customers have high CLV
Lost customers are not profitable to target heavily

---

## **Recommendation**

Champions: Retain with exclusive value offers.  
Loyal: Strengthen through rewards and cross-sell.  
Potential: Convert with onboarding and targeted offers.  
At Risk: Recover with win-back strategies.  
Needs Attention: Encourage repeat purchases with incentives.  
Lost: Low-cost outreach only; avoid high marketing spend.  
Overall: Focus marketing budget on high-value segments.

---
## **Tech Stack**

Python (pandas, numpy, matplotlib, seaborn)
SQL (segmentation, scoring, aggregation)
Power BI (dashboard creation)
Jupyter Notebook for EDA and modeling

---

## **Conclusion**

This project represents a complete, end-to-end Data Analyst workflow.  
It covers:
- data ingestion  
- SQL-based data modeling  
- data cleaning and transformation  
- RFM metric creation and segmentation  
- CLV feature engineering  
- dashboard reporting

The output enables the business to identify high-value segments, reduce churn risk, improve retention strategy, and optimize marketing investments through data-driven customer intelligence.

---


## **Author**
Priyanka Lakra
Aspring Data Analyst | SQL | Python | Power BI
Focused on solving business problems using analytics.

