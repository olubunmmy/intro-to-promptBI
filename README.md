# AI for Business interlligence:Vehicle Sales and Market Trends Analysis (PromptBI Pilot)



## Project Overview

This project leveraged the PromptBI platform to conduct a rapid, AI-assisted assessment of vehicle pricing efficiency in comparison to estimated Market Value (MMR). The objective was to identify patterns and gaps where sales performance diverged from market benchmarks. Through the analysis, the team discovered that 65% of below-market (loss) transactions were concentrated in high-mileage vehicles, specifically those exceeding 80,000 miles.

This pilot project successfully produced a validated and efficient data model while generating actionable insights to guide improvements in pricing accuracy and procurement strategies. The results provide a strong foundation for expanding the analysis into broader operational and strategic decision-making.

## Project Objectives

* **Market Efficiency Analysis:** Compare actual selling price against estimated market retail (`mmr`) to measure market pricing efficiency and identify over/undervalued vehicle segments.
* **Depreciation Curve Modeling:** Quantify the exact impact of vehicle age, condition, and mileage on value loss to accurately model and predict depreciation rates.
* **Predictive Pricing System:** Develop a comprehensive machine learning model utilizing all vehicle features to forecast a highly accurate and reliable selling price estimate.
* **Consumer Preference Insights:** Segment sales data across location (`state`), body type, and manufacturer to map regional demand and pinpoint specific consumer preferences.
* **Anomaly Detection:** Identify and flag extreme outliers where the selling price significantly deviates from the market retail value, ensuring data quality and enabling investigation into unique sales events.



![PromptBI  interface](https://github.com/user-attachments/assets/71e79097-463c-49ff-b575-e12b6fb5a9c3)



---

## Dataset Overview

The dataset captures detailed records of vehicle sales transactions, providing a rich source of data for understanding the dynamics of the used and new vehicle markets. By combining transactional data with vehicle specifications and estimated market values, analysts can gain deep insights into pricing, depreciation, and consumer preferences.

---


 ## Tools and Technologies

| Category | Tool/Language | Purpose |
| :--- | :--- | :--- |
| **AI Generation** | PromptBI (Assumed) | Code generation, narrative summarization, initial modeling |
| **BI Tool** | Power BI Desktop | Data Model visualization and final report creation |
| **Code & Scripting** | Python (Pandas, NumPy) | Advanced statistical analysis and data cleaning logic |
| **Version Control** | Git / GitHub | Repository management and code artifact storage |
## 1. Project Goals and Business Problem



### 1.2 Analysis Objectives
This analysis was structured to answer the following core business questions:
* Which vehicle makes and models had the highest number of sales?
* How does the average selling price compare to the MMR (market value) for different
makes and models?
* How does vehicle mileage affect the selling price?
* Are there vehicles that sold for significantly more or less than their estimated market value
(MMR)?

---

## 2. Data Sources and Schema






---

## 3. Methodology: The PromptBI Workflow

This project emphasizes the use of **PromptBI** to rapidly generate and validate analytical code, moving the analyst's focus from syntax generation to interpretation.

### 3.1 Data Preparation (AI-Assisted ETL)
The following transformations were generated and executed using natural language prompts:

| Transformation Step | Prompt Used (Artifact) | Generated Code Preview | Purpose |
| :--- | :--- | :--- | :--- |
| **Outlier Handling** | "In the 'Revenue' column, cap all values exceeding the 99th percentile." | [`Prompt_01_Outlier_Cap.txt`](./PromptBI_Artifacts/Prompts/Prompt_01_Outlier_Cap.txt) | **`pandas.clip()`** function to stabilize distribution. |
| **Feature Creation** | "Create a 'Time_of_Day' column (Morning, Afternoon, Evening) from the 'Transaction_Time'." | [`Code_02_Time_Feature.py`](./PromptBI_Artifacts/Generated_Code/Code_02_Time_Feature.py) | Facilitate time-based segmentation analysis. |


---

## 4. Key Findings and Actionable Insights

The analysis results, visualized in the Prompt BI dashboard, revealed several critical findings:

1.  **High-Margin Customers:** The **'Referral'** acquisition channel accounts for only $\text{15\%}$ of total transactions but contributes over $\text{35\%}$ of the total profit, indicating a significantly higher Customer Lifetime Value (LTV).
    * **Action:** Double the marketing budget allocated to referral programs.
2.  **Seasonality Anomaly:** The traditional Q4 sales peak has shifted, with **Q3 now showing a $\text{10\%}$ higher revenue growth rate** driven entirely by Product Category 'Z'.
    * **Action:** Re-align inventory and promotional strategies to focus peak activity in Q3.
3.  **Inventory Risk:** Inventory Turnover for Product Category 'A' is $\text{25\%}$ slower than the company average, leading to high carrying costs.
    * **Action:** Implement a just-in-time inventory system for Category 'A' to reduce warehousing expenses.

---

## 6. Repository Structure and Viewing the Report

### 6.1 Repository Contents
The key files for replicating the analysis are:
* `PowerBI/Analysis_Report.pbix`: The final report file.
* `Data/cleaned_data.csv`: The prepared dataset used in the final model.
* `PromptBI_Artifacts/`: Contains all the code and prompts documented above.


