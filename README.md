# Strategic Loan Insights & Risk Monitoring

## Overview
The Bank Loan Analytics Project is a full-stack data analysis solution built using SQL, Power BI, Python, Excel, and Tableau. The project focuses on understanding bank loan performance, identifying high-risk areas, and delivering strategic business insights.This report aims to provide stakeholders with actionable insights into loan applications, approvals, and related metrics.

## Data Source
The data is sourced from internal banking systems and exported as .csv. It contains detailed records on loan applications, borrower demographics, financial ratios, and repayment behavior.

## Tools & Technologies

                                                          
 **SQL (MySQL / SQL Server)** :              Data cleaning, transformation, and KPI calculation                    
 **Power BI** :                               Executive and operational dashboards with real-time interactivity     
 **Python (Pandas, Seaborn, Matplotlib)**:    EDA, correlation analysis, outlier detection                          
 **Excel** :                                  Quick checks, pivot tables, and light dashboards for offline users    
 **Tableau**:                                 Visually compelling dashboards with rich interactivity and storylines 

### Data Fields and Usage
The data utilized in the dashboards comprise several fields, each serving a specific purpose in loan management and risk assessment:

* Loan ID: Unique identifier for loans.
* Address State: Borrower location for regional analysis.
* Employment Length: Indicates - employment stability.
* Employee Title: Job title for income source verification.
* Grade/Sub Grade: Creditworthiness and risk classification.
* Home Ownership: Housing status for financial stability assessment.
* Issue Date: Loan origination date.
* Loan Status: Current state of the loan for performance tracking.
* Purpose: Loan reason for segmentation and customization.
* Term: Loan duration.
* Verification Status: Status of financial information verification.
* Annual Income: Yearly earnings for creditworthiness.
* DTI: Debt burden relative to income.
* Instalment: Monthly repayment amount.
* Interest Rate: Cost of borrowing.
* Loan Amount: Principal amount borrowed.
* Each field plays a crucial role in managing loans, assessing borrower risk, structuring loan terms, and making informed lending decisions.

 ### Implementation Steps
#### 1. Data Preparation
* Loaded .csv into SQL Server using LOAD DATA or GUI import.
* Cleaned nulls, fixed formats, normalized categorical values.

#### 2. SQL Transformations
* Created views for:
* KPI Summary
* Risk Segments (DTI buckets, Grades)
* Temporal Aggregations
* Used CASE, JOIN, GROUP BY, and window functions.

#### 3. Python EDA
* Connected data Source
* Explored distributions, anomalies, and generated insight visuals.

#### 4. Power BI Modeling
* Imported Data From CSV File.
* Defined measures using DAX (e.g., MoM Growth, Risk Ratio).
* Built dashboards with slicers and bookmarks.

#### 5. Tableau Storytelling
* Connected to SQL and .csv files.
* Used Calculated Fields, Level of Detail (LOD), and interactive filters.
* Created drill-downs for Grade → State → Loan Purpose → Borrower Risk.

#### 6. Excel Dashboarding
* Pivoted metrics with slicers.
* Used conditional formatting for red flags (e.g., High DTI & Low Income).
* Enabled snapshot analysis for non-technical users.

### Data Validation Strategy

**SQL Query Verification**: Manually reviewed output for each KPI.
**Python Double Check**: Plotted summary statistics and ensured alignment.
**Power BI DAX Testing**: Used CALCULATE() and FILTER() to mimic SQL logic.
**Tableau Data Interpreter**: Validated with SQL output via custom calculated fields.
**Excel Cross-checking**: Compared pivot values to SQL exports.

### Conclusion
This project exemplifies the power of combining tools for data excellence. It:

* Automates insights using SQL.
* Visualizes strategically using Power BI and Tableau.
* Analyzes deeply with Python.
* Simplifies access with Excel.

The result is a complete 360° view of bank loan operations, borrower risk profiles, and growth metrics — enabling smarter, faster, and more confident decisions across departments.
