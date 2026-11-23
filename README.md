# Retail Revenue & Customer Intelligence
### A Python Data Analysis Project

A Python-based retail data analytics project focused on understanding historical revenue performance, customer purchasing behaviour, product contribution, geographical distribution and invoice patterns using the **Online Retail II** dataset.

## Project Overview

This project analyses more than one million historical retail transaction records from a UK-based online retail business. The analysis uses Python to clean and consolidate transaction data, investigate data quality, calculate revenue, identify business patterns and generate customer insights.

The project follows a structured analytical workflow, from initial data assessment to exploratory data analysis, RFM customer segmentation and final integrity validation.

## Objectives

- Assess and prepare the original retail transaction data.
- Analyse overall revenue and monthly performance.
- Identify products contributing the highest recorded revenue.
- Examine customer purchasing behaviour and revenue concentration.
- Apply RFM analysis for customer segmentation.
- Analyse geographical and invoice-level performance.
- Investigate missing values, negative transactions and zero-revenue records.
- Validate the consistency of analytical results.

## Tools & Technologies

- **Programming:** Python
- **Environment:** Jupyter Notebook
- **Data Analysis:** Pandas, NumPy
- **Data Visualisation:** Matplotlib, Seaborn
- **Techniques:** Data Cleaning, EDA, Revenue Analysis, RFM Segmentation, Pareto Analysis, Trend Analysis and Data Validation

## Dataset Information

**Dataset:** Online Retail II  
**Source:** UCI Machine Learning Repository  
**Original Dataset Creator:** Daqing Chen  
**Period Covered:** 1 December 2009 – 9 December 2011  
**Original Format:** Excel Workbook

[Access the Online Retail II Dataset](https://archive.ics.uci.edu/dataset/502/online+retail+ii)

The original workbook contains two worksheets. After investigating overlapping date coverage and consolidating the records, the working dataset contained **1,044,848 rows and 15 columns**.

The original dataset is not included in this repository because of its file size. Please download it from the official UCI source before running the notebook.

## Project Workflow

1. Dataset loading and initial inspection
2. Data quality assessment
3. Worksheet consolidation and overlap investigation
4. Missing-value and duplicate-record analysis
5. Revenue calculation using Quantity × Price
6. Exploratory data analysis
7. Monthly revenue and trend analysis
8. Product and customer performance analysis
9. RFM customer segmentation
10. Country and invoice-level analysis
11. Pareto revenue concentration analysis
12. Final integrity checks

## Key Findings

| Metric | Result |
|---|---:|
| Consolidated transaction records | 1,044,848 |
| Distinct invoices | 53,628 |
| Identifiable customers | 5,942 |
| Positive line revenue | £20,534,115.49 |
| Negative line revenue | -£1,624,353.37 |
| Net line revenue | £18,909,762.12 |
| Zero-revenue transaction lines | 6,024 |

### Additional Insights

- November 2011 recorded the highest monthly net line revenue at **£1,461,756.25**.
- Regency Cakestand 3 Tier ranked highest among the analysed product combinations, with **£314,513.47** in net line revenue.
- The Champions RFM segment contained **1,275 customers** and contributed **£11,408,916.30** in net line revenue.
- The final integrity audit successfully passed all **17 validation checks**.

## Important Data Limitations

- Customer ID was missing in approximately 22.52% of the consolidated records.
- Product descriptions were missing in 4,275 records.
- Customer-level analysis represents only records with identifiable customer IDs.
- Net line revenue is not equivalent to profit because complete cost information is unavailable.
- Negative revenue should not automatically be interpreted as a confirmed refund.
- The dataset is historical and does not establish present-day customer behaviour or predict future sales.

## Repository Contents

- `Retail_Revenue_Customer_Intelligence_Final.ipynb` — Main Python analysis notebook.
- `RETAIL_REVENUE_REPORT.docx` — Detailed project report.
- `requirements.txt` — Required Python libraries.
- `data/` — Dataset instructions.
- `screenshots/` — Project visualisations and dashboard screenshots.

## How to Run the Project

1. Clone or download this repository.
2. Download the Online Retail II Excel workbook from the official UCI source.
3. Place the workbook in the appropriate data location and ensure its filename and notebook file path match.
4. Install the required libraries:

   ```bash
   pip install -r requirements.txt
   ```

5. Open Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

6. Open the project notebook and execute the cells in sequence.

## Project Purpose

This project demonstrates the practical application of Python-based data analytics to a real-world retail dataset. It combines data preparation, analytical techniques and business interpretation to convert historical transaction records into meaningful insights.

---

**Dataset Attribution:** Online Retail II dataset by Daqing Chen, UCI Machine Learning Repository. Distributed under the Creative Commons Attribution 4.0 International (CC BY 4.0) licence.
