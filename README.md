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



---

## Dataset Overview

The dataset captures detailed records of vehicle sales transactions, providing a rich source of data for understanding the dynamics of the used and new vehicle markets. By combining transactional data with vehicle specifications and estimated market values, analysts can gain deep insights into pricing, depreciation, and consumer preferences.

---


 ## Tools and Technologies

| Category | Tool/Language | Purpose |
| :--- | :--- | :--- |
| **AI Generation** | PromptBI (Assumed) | Code generation, narrative summarization, initial modeling |
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
(MMR)
---

## 3. Methodology: The PromptBI Workflow

This project emphasizes the use of **PromptBI** to rapidly generate and validate analytical code, moving the analyst's focus from syntax generation to interpretation.

### 3.1 Data Preparation (AI-Assisted ETL)
The following transformations were generated and executed using natural language prompts:


![PromptBI  interface](https://github.com/user-attachments/assets/154f419d-738b-4a6a-8c36-40ae21ca1465)


---

## 4. Key Findings and Actionable Insights

The analysis results, visualized in the Prompt BI dashboard, revealed several critical findings:

### **Highest Number of Sales by Make and Model:** 
The Nissan Altima leads in sales with a total of 19,349 units sold. This is highlighted in the chart showing the top 15 make/model combinations by sales count.
    
1.  **Market Value Comparison:** Average selling prices for top models should be compared to their MMR to identify discrepancies.
This comparison can reveal opportunities for pricing strategies or highlight market inefficiencies.

    
2.  **Mileage Impact on Selling Price:** Analyzing how mileage affects selling price can inform inventory management and customer expectations.
Lower mileage vehicles typically command higher prices, which can be leveraged in marketing efforts.

3.**Deviations from Market Value:** Identify vehicles sold significantly above or below MMR to understand market dynamics or customer perceptions.
Such deviations can indicate brand loyalty, unique vehicle features, or market saturation.



![Top Make](https://github.com/user-attachments/assets/7e71baef-8a9f-4058-b0f4-49040e7336dd)


![Make and model](https://github.com/user-attachments/assets/67512eea-20cb-4669-bb29-9d724a49e4b2)


