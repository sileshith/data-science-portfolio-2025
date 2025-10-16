
## **Business Analytics with Excel - Sample Superstore Sales Dataset**

### **Overview**

This project applies end-to-end data analysis techniques in Microsoft Excel, including **Descriptive Statistics, A/B Testing, ANOVA, Regression, and Forecasting**, to demonstrate structured business decision-making using real-world data.

The analysis reflects foundational learning outcomes from the **Data Science (Business Analytics Track)** program at **Arizona State University**, bridging mathematical reasoning with applied business strategy.


### **1. Objective**

To analyze real-world retail data using Excel’s analytical and statistical tools, identifying insights that drive **profit optimization, pricing discipline, and operational efficiency**.

This analysis explores how data-driven insights support **marketing, sales, and regional business decisions**, from exploratory statistics to predictive modeling and forecasting.


### **2. Dataset**

**Name:** Sample Superstore Sales Dataset
**Source:** [Tableau Community — Sample Superstore Excel File](https://community.tableau.com/s/question/0D54T00000G551cSAB/sample-superstore-sales-excelxls)
**Format:** Microsoft Excel (.xls)

**Description:**
The dataset simulates retail operations for an office supply and furniture company across the United States.
It includes:

* **Order information:** Order ID, Date, Ship Mode, Customer Segment
* **Product details:** Category, Sub-Category, Product ID, Product Name
* **Sales metrics:** Sales, Quantity, Discount, Profit
* **Geography:** Country, State, Region, and City

I chose this dataset for demonstrating analytical reasoning and business insight through Excel-based testing, modeling, and forecasting.


### **3. Analytical Techniques**

| **Method**                    | **Excel Tool**                      | **Purpose**                                              |
| ----------------------------- | ----------------------------------- | -------------------------------------------------------- |
| **Descriptive & Correlation** | Data Analysis ToolPak               | Summarize data distribution and relationships            |
| **A/B Testing (t-Test)**      | ToolPak: t-Test (Unequal Variances) | Compare performance between two business groups          |
| **ANOVA**                     | ToolPak: ANOVA: Single Factor       | Compare mean sales or profits across multiple categories |
| **Regression**                | ToolPak: Regression                 | Predict Profit using Sales, Discount, and Quantity       |
| **Forecasting**               | FORECAST.LINEAR / Moving Average    | Estimate future sales trends over time                   |


### **4. Descriptive Statistics**

**Goal:** Identify key distribution patterns in Sales, Profit, Discount, and Quantity.  
**Tool:** Analysis ToolPak → Descriptive Statistics & Correlation.

**Findings:**

* **Sales & Profit:** Highly right-skewed; a few large orders dominate total revenue.
* **Discount:** Wide range (0–80%); high kurtosis signals deep-discount outliers.
* **Quantity:** Relatively stable (1–5 units typical), implying limited volume variability.
* **Correlation:** Sales–Profit (r = +0.48), Discount–Profit (r = –0.22) → deeper discounts lower margins.

**Business Interpretation:**
Focus pricing strategy on sustainable margins rather than high-volume, low-profit sales.
Flag high-discount transactions for managerial review to minimize profit erosion.


### **5. Pivot Table Analysis**

**A. Sales and Profit by Category and Region**

* *Technology* drives highest profit growth; *Furniture* underperforms relative to volume.
* *West Region* dominates both sales and profitability; *Central* shows margin compression.
  **Recommendation:** Prioritize West and East for growth initiatives; improve Central’s cost control and logistics efficiency.

**B. Customer Segment vs. Discount**

* *Consumer* segment receives higher discounts than *Corporate* or *Home Office*.
  **Recommendation:** Adjust Consumer discount tiers and implement a standardized discount approval process to stabilize margins.

**C. Monthly Sales Trend by Ship Mode**

* *Standard Class* leads order volume; *Same-Day* peaks around seasonal demand spikes.
  **Recommendation:** Scale shipping resources during forecasted peaks; review Same-Day profitability for efficiency optimization.


### **6. A/B Testing**

#### **Purpose**

To statistically compare key business segments and identify differences in profitability and discount behavior.

| **Test**                                | **Groups (A/B)**            | **Metric Tested**                   | **Result**                                               | **Business Decision**                                                                   |
| --------------------------------------- | --------------------------- | ----------------------------------- | -------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| **A/B Test 1: East vs. West (Primary)** | East Region vs. West Region | Profit per Order                    | Significant difference (p < 0.05)                        | Replicate West region’s pricing and logistics strategy in East; review East’s sales mix |
| **A/B Test 2: Consumer vs. Corporate**  | Customer Segment            | Average Discount & Profit per Order | Consumers receive higher discounts without higher profit | Narrow discount range for Consumer segment; focus on profit-based promotions            |
| **A/B Test 3: Low vs. High Discount**   | ≤ 20% vs. > 20% Discount    | Profit per Order                    | High-discount orders yield lower average profit          | Implement 20% discount cap; require approval above threshold                            |

#### **Conclusion**

Among all tests, **East vs. West Profit Comparison** was selected as the **primary high-impact A/B test**.
It ties directly to regional operations, balanced group sizes, and actionable strategy outcomes that affect resource allocation, marketing, and supply chain optimization.


### **7. ANOVA - Comparing Mean Sales Across Categories**

**Objective:** Determine if product categories differ significantly in mean order value.
**Tool:** ToolPak → ANOVA: Single Factor.
**Result:** p < 0.05 → mean sales differ significantly across categories.
**Interpretation:** Technology category generates higher sales per order. 
**Recommendation:** Expand Technology portfolio and prioritize high-value inventory.


### **8. Regression Analysis - Profit Drivers**

**Model:** Profit = β₀ + β₁(Sales) + β₂(Discount) + β₃(Quantity)
**Tool:** ToolPak → Regression Analysis.
**Results:**

* **Sales:** positive and significant driver of profit.
* **Discount:** negative coefficient; deeper discounts reduce profit.
* **Quantity:** small positive contribution.
* **R² ≈ 0.65:** model explains ~65% of profit variability.

**Recommendation:**
Limit discounts to maintain profit margins; focus on high-sales, low-discount items for sustainable growth.


### **9. Forecasting**

**Goal:** Predict near-term sales using time-based trends.  
**Tool:** FORECAST.LINEAR / 3-Month Moving Average.  

**Findings:**

* Monthly sales show cyclical peaks mid-year.
* Clear upward trend over time.

**Recommendation:**
Plan marketing campaigns and inventory buildup around predictable seasonal surges.  
Use a rolling 3-month forecast to guide staffing and replenishment schedules.


### **10. Expected Deliverables**

* **Excel Workbook** containing:

  * Cleaned and formatted dataset
  * Descriptive statistics and correlation outputs
  * A/B Testing, ANOVA, and Regression analysis sheets
  * Forecasting worksheet with visual trendlines
  * PivotTable-based interactive dashboard
* **Documentation** (README and PDF summary) explaining:

  * Statistical results
  * Business interpretations and recommendations



### **11. Skills Demonstrated**

* Advanced Excel analytics (Analysis ToolPak, PivotTables, Forecasting)
* Statistical hypothesis testing (t-Test, ANOVA)
* Regression modeling for profit optimization
* Forecasting using moving averages and trendlines
* Business storytelling and visualization
* Executive communication of data-driven insights



#### **Outcome**

This project demonstrates a complete analytical workflow using Excel, from data preparation to actionable business recommendations.
It connects statistical analysis with operational decision-making - **transforming descriptive metrics into strategic insights**.

Key outcomes:

* Quantified profit impact of discounts and regional operations.
* Established evidence-based discount caps and regional focus.
* Created forecasting tools to support seasonal business planning.



#### **Author**  
**Sileshi T. Hirpa**. 
Data Science (Business Analytics Track) — *Arizona State University*. 
  San Francisco Bay Area, CA  
 [hirpast@gmail.com](mailto:hirpast@gmail.com). 
 [LinkedIn Profile](https://www.linkedin.com/in/sileshi-hirpa). 

