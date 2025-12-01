# AI for Business intelligence:Vehicle Sales and Market Trends Analysis (PromptBI Pilot)



## Project Overview

This project leveraged the PromptBI platform to conduct a rapid, AI-assisted assessment of vehicle pricing efficiency in comparison to estimated Market Value (MMR). The objective was to identify patterns and gaps where sales performance diverged from market benchmarks.

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

**Business Implications:**
Focus marketing and sales efforts on high-demand models like the Nissan Altima.
Conduct deeper analysis on price vs. MMR to optimize pricing strategies.
Use mileage data to better position vehicles in the market and manage expectations.


### Average Selling Price vs MMR by Make and Model
The analysis reveals that the Ford F-150 has the largest gap between the average selling price and MMR, with a difference of $218.76. This indicates a notable variance in market perception versus actual selling price.


<img width="1253" height="554" alt="image" src="https://github.com/user-attachments/assets/b65b9757-bcf6-46a3-8baf-23b9164b0603" />

1. **Sales Gap Analysis:**
The largest gap in sales is observed for the Ford F-150 with a difference of 218.76 units. This significant gap suggests either exceptional performance or a potential market anomaly worth investigating.

3. **Implications for Business Strategy:**
- Focus on High-Demand Models: Given the Ford F-150's strong sales, consider increasing inventory and marketing efforts for this model. - Investigate Sales Gaps: Analyze the reasons behind the large sales gap for the Ford F-150 to replicate success or address underlying issues.

  **Action:**
-Conduct a deeper dive into the sales data for the Ford F-150 to understand contributing factors.
-Review market conditions and competitor strategies to align with the high demand for this model.
-Consider targeted promotions or bundles to further boost sales of the Ford F-150.

###  Vehicle Mileage vs Selling Price
There is a significant negative correlation between vehicle mileage and selling price, with a correlation coefficient of -0.58. This suggests that as the odometer reading increases, the selling price tends to decrease.

![odometer](https://github.com/user-attachments/assets/ce761e6e-9e1b-4628-b831-e4b647127fab)


### Insights from Vehicle Sales Data

1. **Highest Number of Sales by Vehicle Makes and Models**
Insight: The chart does not provide specific data on vehicle makes and models with the highest number of sales. Further segmentation is required to identify top-selling vehicles.
2. **Average Selling Price vs. MMR (Market Value)**
Insight: The chart lacks detailed comparison data between average selling prices and MMR for different makes and models. Additional data collection is needed to perform this analysis.
3. **Vehicle Mileage Impact on Selling Price**
Insight: The chart shows a wide range of odometer readings from 0 to 999,999 miles and selling prices from $100 to $88,000.
Generally, higher mileage tends to correlate with lower selling prices.
However, specific trends require deeper analysis with more granular data.

4. **Vehicles Sold Significantly Above or Below MMR**
Insight: The chart does not provide enough data to identify vehicles sold significantly above or below their estimated market value (MMR). More detailed pricing and MMR data are necessary for this analysis.

**Next Steps**
-Collect detailed sales data segmented by vehicle make and model.
-Gather MMR data for accurate comparison with selling prices.
-Analyze the relationship between mileage and selling price with a larger dataset.

4. **Vehicles Sold Significantly Above or Below MMR**
The Nissan Altima again stands out, with 3,274 vehicles sold significantly above MMR and 3,591 sold significantly below. This indicates a wide variance in pricing for this model.


![above and below](https://github.com/user-attachments/assets/f874d2d4-fed4-4f18-8d77-c6dac62327ba)

 ## Conclusion
1. **Highest Number of Sales**
The Nissan Altima has the highest number of significant price deviations, indicating a strong presence in the market.

2. **Price Deviations from MMR**
The Nissan Altima shows the most instances of both above and below market value (MMR) sales.
Above MMR: 3274 instances
Below MMR: 3591 instances

3. **Implications for Business**
The high number of deviations for the Nissan Altima suggests variability in pricing strategies or market conditions.
This could indicate opportunities for targeted marketing or pricing adjustments to better align with market values.

4. **Recommended Next Move**
Investigate the causes behind the significant price deviations for the Nissan Altima.
Consider refining pricing strategies to reduce the gap between selling price and MMR.

System Message Note: While the analysis provides valuable insights, it’s important to note that some data might be sampled or filtered for clarity. For the most accurate results, consider analyzing the complete dataset or specific segments of interest.
If you have any specific makes or models you’d like to dive deeper into, feel free to ask!




