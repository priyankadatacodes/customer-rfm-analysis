# **Customer RFM Segmentation Project**
![SQL](https://img.shields.io/badge/SQL-MySQL-orange) →![Python](https://img.shields.io/badge/Python-3.10%2B-blue)→![Power BI](https://img.shields.io/badge/BI-Power%20BI-yellow)

This project showcases an end-to-end Customer RFM Segmentation and CLV analysis project built using SQL (MySQL), Python (Pandas, SQLAlchemy), and Power BI. The complete workflow demonstrates real data analyst responsibilities, including data ingestion, cleaning, modeling, SQL-based segmentation, CLV enrichment, and analytical reporting.

<img src="https://raw.githubusercontent.com/priyankadatacodes/customer-rfm-analysis/main/workflowdiagram.png" width="100%">


---

## **Business Problem**

The business treats all customers uniformly without understanding their value contribution, purchase frequency, or monetary potential. As a result, marketing investments are inefficient, retention efforts are misaligned, and dormant customers remain unidentified.

To resolve this, the company requires a segmentation model that classifies customers based on their purchasing behavior and revenue patterns. RFM-based segmentation combined with CLV analytics helps detect:
- high-value customers,
- loyal repeat buyers,
- potential growth candidates,
- at-risk customers,
- lost or inactive customers.

The outcome enables targeted campaigns, optimized discount strategies, revenue forecasting, and improved decision-making.

---

## **Project Objective**

- Implement RFM analysis on customer transactional data  
- Assign NTILE-based scores to Recency, Frequency, and Monetary metrics  
- Classify customers into strategic behavioral groups  
- Enrich RFM output with CLV and retention indicators  
- Deliver final dataset for BI dashboard insights and decisions  

---

## **End-to-End Workflow**

SQL → Python → SQL → Python → Power BI

1. Database setup and raw table schema  
2. Raw data import, cleaning, transformation and creation of final table  
3. SQL-based RFM metric calculation and customer segmentation  
4. Python-based CLV computation and final enriched dataset  
5. Power BI dashboard for business insights  

---

## **Project Implementation (Based on Actual Files)**

### **1. SQL: Database & Table**
**File:** `01_rfm_database_and_table_creation.sql`  
Tasks performed:
- Created database `rfm_project`
- Designed `orders_raw` schema for raw data  

This sets the foundation for transactional storage and subsequent processing.

---

### **2. Python: Data Load, Cleaning & Final Table Creation**
**File:** `02_python_cleaning.ipynb`  
Operations performed:
- Loaded CSV into pandas  
- Checked datatypes and nulls  
- Removed missing CustomerIDs  
- Converted CustomerID to numeric  
- Filled missing product descriptions  
- Removed negative quantity and unit price rows  
- Created `TotalPrice` column  
- Push cleaned data into MySQL table `orders_clean`

This ensures a reliable and analysis-ready dataset.

---

### **3. SQL: RFM Metrics & Segmentation**
**File:** `03_rfm_modeling.sql`  
RFM Logic Implemented:
- Recency (days since last purchase)  
- Frequency (unique invoices)  
- Monetary (total spend)  
- NTILE(5) scoring for R, F, M metrics  
- Final RFM score (concatenated code)  
- Segment assignment:
  - Champions
  - Loyal Customers
  - Potential
  - At Risk
  - Lost
  - Needs Attention

Tables generated:
- `rfm_table`
- `rfm_scores`
- `rfm_final`

This step performs complete segmentation using pure SQL logic.

---

### **4. Python: Final Fetch, CLV Features & Export**
**File:** `04_rfm_analysis.ipynb`  
Key enrichments:
- Active customer months  
- Purchases per month  
- Average order value  
- 12-month CLV projection  
- Final merged dataset export (`final_rfm_output.csv`)

This enhances segmentation with value-based business indicators.

---

### **5. Power BI: Dashboard**
BI visuals built on the enriched dataset:
- RFM segment distribution  
- Revenue share by segment  
- CLV projections  
- Frequency & monetary patterns  

Supports strategic decisions on retention and customer targeting.

---

## **Final Output Dataset**

Output File:
`final_rfm_output.csv`

Includes:
- RFM metrics  
- R, F, M scores  
- Final RFM code  
- Customer segment  
- Active months  
- Monthly buying frequency  
- Average order value  
- CLV (12 months)

This final dataset is used for BI reporting.

---

## **Key Insights Delivered**

- Champions and Loyal segments contribute the highest monetary share  
- Lost customers show long inactivity windows  
- Potential customers are suitable for upselling  
- CLV reveals top revenue generators  
- RFM segmentation enables selective discounting instead of blanket offers  

These insights support informed retention, targeting, and marketing budgets.

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


---

## **Author**
By Priyanka Lakra


