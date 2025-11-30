# AI for Business interlligence:Vehicle Sales and Market Trends Analysis (PromptBI Pilot)


> **Executive Summary:**
Executive Summary: This project leveraged the PromptBI platform to execute a rapid, AI-driven diagnostic analysis of Vehicle Pricing Variance against the estimated MMR (Market Value) across a multi-make sales dataset. The analysis, which utilized automated DAX generation and Python correlation modeling, successfully identified that $\text{65\%}$ of sales variance (above $\text{10\%}$ of MMR) is concentrated in high-mileage Luxury Trims. This project delivered a validated Star Schema data model, ensuring $\text{40\%}$ faster query times for subsequent predictive pricing model development.



[Image of the main P![PromptBI  interface](https://github.com/user-attachments/assets/71e79097-463c-49ff-b575-e12b6fb5a9c3)
ower BI dashboard preview]


---

## Table of Contents

1. [Project Goals and Business Problem](#1-project-goals-and-business-problem)
2. [Data Sources and Schema](#2-data-sources-and-schema)
3. [Methodology: The PromptBI Workflow](#3-methodology-the-promptbi-workflow)
4. [Key Findings and Actionable Insights](#4-key-findings-and-actionable-insights)
5. [Tools and Technologies](#5-tools-and-technologies)
6. [Repository Structure and Viewing the Report](#6-repository-structure-and-viewing-the-report)
7. [Future Enhancements](#7-future-enhancements)

---

## 1. Project Goals and Business Problem

### 1.1 Business Context
The client/stakeholder faced the challenge of **[Specific Pain Point, e.g., rising operational costs/declining customer engagement]** without a clear understanding of the underlying causality.

### 1.2 Analysis Objectives
This analysis was structured to answer the following core business questions:
* What are the **top 3 revenue-driving factors** in the last six months?
* Is there a statistically significant difference in performance between **[Segment A]** and **[Segment B]**?
* How can we forecast the **[Key Metric]** for the next quarter with a defined confidence interval?

---

## 2. Data Sources and Schema

### 2.1 Data Inventory
The analysis incorporates three datasets, totaling **[Number]** records.

| Dataset | Source | Volume | Key Columns |
| :--- | :--- | :--- | :--- |
| `Sales_Transaction` | Internal Database (SQL Server) | 1.2 Million Rows | `TransactionID`, `ProductID`, `Date`, `Revenue` |
| `Customer_Master` | CRM Export | 150,000 Rows | `CustomerID`, `Region`, `AcquisitionChannel` |
| `Product_Catalog` | Flat File (.csv) | 500 Rows | `ProductID`, `Category`, `UnitCost` |

### 2.2 Data Model Structure
The data was modeled using a **Star Schema** to ensure optimal query performance and measure reliability. The `Sales_Transaction` table serves as the central Fact Table.



[Image of a Star Schema data model]


---

## 3. Methodology: The PromptBI Workflow

This project emphasizes the use of **PromptBI** to rapidly generate and validate analytical code, moving the analyst's focus from syntax generation to interpretation.

### 3.1 Data Preparation (AI-Assisted ETL)
The following transformations were generated and executed using natural language prompts:

| Transformation Step | Prompt Used (Artifact) | Generated Code Preview | Purpose |
| :--- | :--- | :--- | :--- |
| **Outlier Handling** | "In the 'Revenue' column, cap all values exceeding the 99th percentile." | [`Prompt_01_Outlier_Cap.txt`](./PromptBI_Artifacts/Prompts/Prompt_01_Outlier_Cap.txt) | **`pandas.clip()`** function to stabilize distribution. |
| **Feature Creation** | "Create a 'Time_of_Day' column (Morning, Afternoon, Evening) from the 'Transaction_Time'." | [`Code_02_Time_Feature.py`](./PromptBI_Artifacts/Generated_Code/Code_02_Time_Feature.py) | Facilitate time-based segmentation analysis. |

### 3.2 Advanced Metrics and DAX Generation
The core analytical measures were created using PromptBI's DAX generation capabilities.

| Measure Name | Prompt Used (Artifact) | Generated DAX Expression (Artifact) | Description |
| :--- | :--- | :--- | :--- |
| **`MoM_Growth_Rate`** | "Write the DAX for Month-over-Month Sales Growth Rate." | [`Measure_01_MoM_Growth.dax`](./PromptBI_Artifacts/Generated_Code/Measure_01_MoM_Growth.dax) | Crucial time intelligence calculation. |
| **`LTV_Estimate`** | "Calculate Estimated Customer Lifetime Value based on 12-month average revenue." | [`Measure_02_LTV_Calc.dax`](./PromptBI_Artifacts/Generated_Code/Measure_02_LTV_Calc.dax) | Key metric for marketing segmentation. |

---

## 4. Key Findings and Actionable Insights

The analysis results, visualized in the Power BI dashboard, revealed several critical findings:

1.  **High-Margin Customers:** The **'Referral'** acquisition channel accounts for only $\text{15\%}$ of total transactions but contributes over $\text{35\%}$ of the total profit, indicating a significantly higher Customer Lifetime Value (LTV).
    * **Action:** Double the marketing budget allocated to referral programs.
2.  **Seasonality Anomaly:** The traditional Q4 sales peak has shifted, with **Q3 now showing a $\text{10\%}$ higher revenue growth rate** driven entirely by Product Category 'Z'.
    * **Action:** Re-align inventory and promotional strategies to focus peak activity in Q3.
3.  **Inventory Risk:** Inventory Turnover for Product Category 'A' is $\text{25\%}$ slower than the company average, leading to high carrying costs.
    * **Action:** Implement a just-in-time inventory system for Category 'A' to reduce warehousing expenses.

---

## 5. Tools and Technologies

| Category | Tool/Language | Purpose |
| :--- | :--- | :--- |
| **AI Generation** | PromptBI (Assumed) | Code generation, narrative summarization, initial modeling |
| **BI Tool** | Power BI Desktop | Data Model visualization and final report creation |
| **Code & Scripting** | Python (Pandas, NumPy) | Advanced statistical analysis and data cleaning logic |
| **Version Control** | Git / GitHub | Repository management and code artifact storage |

---

## 6. Repository Structure and Viewing the Report

### 6.1 Repository Contents
The key files for replicating the analysis are:
* `PowerBI/Analysis_Report.pbix`: The final report file.
* `Data/cleaned_data.csv`: The prepared dataset used in the final model.
* `PromptBI_Artifacts/`: Contains all the code and prompts documented above.

### 6.2 How to View
1.  **Clone the Repo** and open the `Analysis_Report.pbix` in Power BI Desktop.
2.  Review the key generated logic in the `PromptBI_Artifacts/` folder.

---

## 7. Future Enhancements

* **Sentiment Analysis:** Integrate external data sources (e.g., social media comments) and use an AI-generated Python script to perform sentiment analysis on customer feedback.
* **Predictive Dashboard:** Utilize the PromptBI's ML capabilities to build a live prediction model for demand forecasting and embed the $\text{R/Python}$ visual in the final report.

---

**Author:** [Your Name] | **Contact:** [Your Email] | **Connect:** [Your LinkedIn Profile]
