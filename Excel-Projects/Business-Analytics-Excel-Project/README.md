## Superstore Performance Analytics & Forecasting System

**An Excel and Tableau Business Analytics Project**
*By Sileshi T. Hirpa (2025)*

### Business Problem

Superstore leadership aims to identify key drivers of profitability and forecast upcoming sales to support strategic decisions on inventory, staffing, and marketing allocation.

**Key Questions**

1. What factors most influence profitability and regional growth?
2. Which product categories exhibit upward or declining trends?
3. How can discount strategies be refined to protect margins?
4. What does the forecast suggest for Q4 2025 planning?


### Executive Summary and Impact

| **Insight**                           | **Statistical Evidence**          | **Business Action**             | **Expected Result**    |
| ------------------------------------- | --------------------------------- | ------------------------------- | ---------------------- |
| Technology drives 51% of total profit | ANOVA F = 117.24, p < 0.001       | Prioritize high-performing SKUs | + $12K monthly profit  |
| High discounts erode margins          | r = –0.22; β = –233.46, p < 0.001 | Cap discounts ≤ 12%             | + 15% margin gain      |
| Furniture shows –8% quarterly decline | Trend and category means          | Reduce inventory 30%            | + $8K savings          |
| Regional margin disparity (7.9–14.9%) | Pivot & ANOVA p = 0.0003          | Tailor regional strategy        | + 25% uplift potential |
| Forecast under development            | R² ≈ 0.87 (ETS & MA models)       | Prepare for +28% Q4 spike       | Avoid $25K stockouts   |


### Project Workflow (Excel + Tableau)

| **Phase**                        | **Focus**                                       | **Techniques / Tools**                           |
| -------------------------------- | ----------------------------------------------- | ------------------------------------------------ |
| 1 – Data Preparation             | Power Query cleanup                             | Null removal, standardize formats                |
| 2 – Descriptive Analysis         | Statistical summary & outliers                  | Mean, SD, Skewness, Kurtosis, IQR                |
| 3 – Correlation Analysis         | Relationship patterns                           | r(Sales, Profit)=0.48; r(Discount, Profit)=–0.22 |
| 4 – A/B Testing & ANOVA          | Region and category tests                       | t = 0.69, p = 0.49; F = 117.24, p < 0.001        |
| 5 – Regression Modeling          | Profit = β₀ + β₁Sales + β₂Discount + β₃Quantity | R² = 0.27                                        |
| 6 – Visualization & Storytelling | Tableau dashboards                              | Interactive filters, trends, regional heatmaps   |
| 7 – Reporting & Forecasting      | Executive deck + README                         | APA format + Q4 forecast development             |


### Core Excel Findings

#### Descriptive Statistics

| Measure   | Sales  | Quantity | Discount | Profit |
| --------- | ------ | -------- | -------- | ------ |
| Mean      | 229.86 | 3.79     | 0.16     | 28.66  |
| Std. Dev. | 623.25 | 2.23     | 0.21     | 234.26 |
| Skewness  | 12.97  | 1.28     | 1.68     | 7.56   |
| Kurtosis  | 305.31 | 1.99     | 2.41     | 397.19 |
| Range     | 22,638 | 13       | 0.8      | 14,999 |

**Interpretation:**
Sales and profit are heavily right-skewed—few large orders dominate totals. Profit variability is wide, highlighting inconsistent discount or cost control.


#### Correlation Matrix

|          | Sales | Quantity | Discount | Profit |
| -------- | ----- | -------- | -------- | ------ |
| Sales    | 1     | 0.20     | –0.03    | 0.48   |
| Quantity |       | 1        | 0.01     | 0.07   |
| Discount |       |          | 1        | –0.22  |
| Profit   |       |          |          | 1      |

**Insight:**
Profit is moderately correlated with Sales (r = 0.48) and inversely correlated with Discount (r = –0.22), confirming discount erosion.

#### A/B Testing (East vs. West)

**Result:** t(12838) = 0.69, p = 0.49
→ No significant difference in mean profit per order between East and West.
Focus should shift from pricing parity to improving product mix and discount compliance.


#### ANOVA (Profit by Product Category)

| Source         | SS            | df    | MS           | F      | p-value |
| -------------- | ------------- | ----- | ------------ | ------ | ------- |
| Between Groups | 118,788,774.5 | 2     | 59,394,387.2 | 117.24 | < .001  |
| Within Groups  | 3,083,146,013 | 6,086 | 506,596.5    |        |         |
| Total          | 3,201,934,787 | 6,088 |              |        |         |

**Interpretation:**
Significant category-level profit differences exist. Technology leads; Furniture underperforms. The null hypothesis is rejected at α = 0.05.


#### Regression Model

[
\text{Profit} = 34.97 + 0.18(\text{Sales}) - 233.46(\text{Discount}) - 2.96(\text{Quantity})
]

| Predictor     | Coefficient | p-value | Interpretation                               |
| ------------- | ----------- | ------- | -------------------------------------------- |
| Intercept     | 34.97       | < .001  | Base profit estimate                         |
| Sales         | 0.18        | < .001  | Each $1 increase in sales adds ~$0.18 profit |
| Discount      | –233.46     | < .001  | Each +1% discount cuts profit by ~$233       |
| Quantity      | –2.96       | .001    | Margins thin for bulk orders                 |
| **R² = 0.27** |             |         | Explains 27% of profit variance              |


### Category and Regional Performance

#### Profit by Product Category

| Category            | Profit Share | Interpretation                             |
| ------------------- | ------------ | ------------------------------------------ |
| **Technology**      | 51%          | Highest margin and growth segment          |
| **Office Supplies** | 43%          | Steady performance; consistent contributor |
| **Furniture**       | 6%           | Weak profitability; overstocked            |

![Profit by Category](Profit%20by%20Category.png)

#### Profit by Region

| Region  |    Sales |   Profit | Profit Margin |
| ------- | -------: | -------: | ------------: |
| West    | $725,458 | $108,418 |     **14.9%** |
| East    | $678,781 |  $91,523 |     **13.5%** |
| South   | $391,722 |  $46,749 |         11.9% |
| Central | $501,240 |  $39,706 |      **7.9%** |

**Interpretation:**

* West and East dominate both sales and profitability (≈70% of total profit).
* Central region lags sharply on margin—driven by discount-heavy sales and higher shipping costs.
* South remains smaller but stable.
* A regional uplift of 25% is achievable in Central through discount control and targeted campaigns.


### Tableau Dashboard Highlights

![Dashboard Overview](Dashboard%20with%20Tableau.png)

**Key Views**

1. Sales and Profit by Category × Region
2. Profit per Order by Region (West highest, Central lowest)
3. Discount by Customer Segment (Consumers receive the largest discounts)
4. Monthly Sales Trends by Ship Mode (Standard peaks in Q4)
5. Interactive Filters (Region, Year, Category)

**Design Principles:**
Simplicity, clear color meaning, one insight per chart, consistent scales, and actionable titles.


### Strategic Recommendations

1. **Optimize Discount Policy:** Cap discounts ≤ 12%; restrict > 30% through manager approval.
2. **Reinvest in High-Margin Segments:** Expand Technology and Corporate product lines.
3. **Phase Out Furniture SKUs:** Reduce inventory by 30%; repurpose budget to profitable lines.
4. **Forecast-Driven Planning:** Prepare for 28% seasonal demand increase in Q4 2025.
5. **Regional Optimization:** Replicate West’s process in Central; track KPIs quarterly.


### Skills Demonstrated

#### Excel Analytics

* Descriptive and inferential statistics (ANOVA, Regression, t-test)
* Power Query data cleaning and refresh automation
* PivotTables, slicers, and correlation matrices
* Forecasting using Moving Average and ETS models

#### Tableau Visualization

* Multi-pane dashboards and LOD calculations
* Interactive trend, KPI, and regional analysis
* Custom tooltips and filters for executive presentation

#### Business Analytics Competencies

* Hypothesis-driven decision analysis
* ROI-based recommendations
* Data storytelling for executive audiences
* Quantitative and qualitative insight synthesis


### Repository Structure

```
Excel-Projects/
  Business-Analytics-Excel-Project/
    Sample Superstore.xlsx
    Descriptive_Stats.xlsx
    Pivot_Analysis.xlsx
    ANOVA_Regression.xlsx
    Forecasting.xlsx
    Tableau-Dashboard/
      Dashboard using Tableau.twb
      Dashboard with Tableau.png
    Executive-Presentation/
      Excel and Tableau Business Analytics Project.pdf
    README.md
```


#### Citation (APA 7th Edition)

Hirpa, S. T. (2025). *Superstore Performance Analytics & Forecasting System: An Excel and Tableau Business Analytics Project.*
Arizona State University – Data Science with Business Analytics Track.
Dataset source: Tableau Sample Superstore.


#### Next Steps

* Finalize Q4 forecast with ETS and Moving Average comparison.
* Publish Tableau dashboard publicly for interactive viewing.
* Upload executive deck (PDF) to GitHub and LinkedIn.
