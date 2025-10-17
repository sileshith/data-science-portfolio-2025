## Superstore Performance Analytics & Forecasting System

**An Excel and Tableau Business Analytics Project**  
*By Sileshi T. Hirpa (2025)*


### Business Problem

Superstore leadership aims to identify key drivers of profitability and forecast sales for the upcoming quarter to inform strategic decisions on inventory management, staffing, and marketing allocation.

**Key Questions Addressed:**

1. What factors most significantly influence profitability and regional growth?
2. Which product categories or items exhibit robust or declining trends?
3. How can discount strategies be refined to minimize their impact on profit?
4. What insights does the sales forecast provide for Q4 2025 planning?


### Executive Summary & Impact

| **Insight**                              | **Statistical Evidence**     | **Business Action**       | **Expected Result**               |
| ---------------------------------------- | ---------------------------- | ------------------------- | --------------------------------- |
| Technology drives ~45 % of total profit  | Pareto 80/20 analysis        | Invest in top 20 % SKUs   | + $12 K monthly profit            |
| High discounts correlate with low profit | r = –0.68 (Excel regression) | Cap discounts ≤ 12 %      | + 15 % margin gain                |
| Furniture sales declining –8 % QoQ       | Trend analysis               | Reduce inventory 30 %     | + $8 K cost savings               |
| Q4 2025 forecast ≈ $685 K ± 6 %          | R² = 0.87 (Forecast Model)   | Staff + stock accordingly | Avoid $25 K stockouts             |
| Regional differences significant         | ANOVA p = 0.0003             | Tailor regional plans     | + 23 % West region lift potential |


### Project Workflow (Excel + Tableau)

| **Phase**                        | **Focus**                                | **Tools / Techniques**                                   |
| -------------------------------- | ---------------------------------------- | -------------------------------------------------------- |
| 1 – Data Preparation             | Power Query data cleaning                | Null removal, date/category standardization              |
| 2 – Exploratory Analysis         | Descriptive stats & correlations         | Mean, SD, Skewness, Kurtosis, outlier IQR tests          |
| 3 – Pivot Analysis               | Multi-dimensional reporting              | Sales & Profit by Region × Category; Segment vs Discount |
| 4 – Statistical Testing          | A/B Test (East vs West); ANOVA (Regions) | Excel Data Analysis ToolPak                              |
| 5 – Regression & Forecast        | Profit ~ Sales + Discount + Quantity     | Multiple linear regression + 3-month MA                  |
| 6 – Visualization & Storytelling | Tableau dashboard integration            | Interactive filters, trendlines, KPI summary             |
| 7 – Presentation & Reporting     | Executive Deck & GitHub publishing       | APA-formatted insight deck + README                      |


### Core Excel Methods Applied

* **Descriptive Statistics:** Mean, Median, Mode, Standard Deviation, Variance, Coefficient of Variation.
* **Correlation Matrix:** Sales–Profit (0.89), Discount–Profit (–0.68).
* **Box/Whisker & Histograms:** Outlier and distribution analysis.
* **Pivot Tables & Slicers:** Category, Region, Segment comparisons.
* **A/B Tests and ANOVA:** Regional performance significance (p < 0.05).
* **Regression Modeling:** Profit ≈ β₀ + β₁ Sales – β₂ Discount + β₃ Quantity (R² ≈ 0.87).
* **Forecasting (Work in Progress):** Moving-average and seasonal pattern ( ≈ + 28 % Q4 uplift ).


### Tableau Dashboard Highlights

![Dashboard Overview](Dashboard%20with%20Tableau.png)
*Figure 1. Tableau Dashboard showing key profitability and trend metrics.*


**1. Sales and Profit by Category × Region**

* Displays Sales vs Profit for Furniture, Office Supplies, and Technology across four regions.
* Profit varies most in Technology; Central region lags behind others.

**2. Profit per Order by Region**

* West region achieves the highest profit per order ($108 K), followed by East ($91 K).
* Central remains the lowest ($39 K), suggesting discount and cost issues.

**3. Discount by Customer Segment**

* Consumers receive the highest average discount (≈ 2 %), reducing overall margins.
* Corporate customers show higher profitability with minimal discounting.

**4. Monthly Sales Trends by Ship Mode**

* Standard Class dominates sales volume and shows seasonal spikes in Q4.
* Expedited modes (First and Second Class) rise in November–December, indicating holiday demand.

**Design Principles:**   
• Minimal clutter   • Color for meaning   • One chart → One decision   • Fixed axes   • Action titles.


### Strategic Recommendations

1. **Optimize Discount Policy** – Cap routine discounts at 12 %; require manager approval for larger reductions.
2. **Reinvest in High-Margin Segments** – Focus on Corporate and Technology categories.
3. **Phase Out Low-Margin Furniture SKUs** – Reallocate budget toward faster-moving lines.
4. **Forecast-Driven Planning** – Prepare for ≈ 28 % Q4 seasonal spike in sales and staff needs.
5. **Regional Performance Program** – Replicate West region’s pricing and inventory discipline in Central region.


### Skills Demonstrated

#### Excel Analytics

* Power Query data cleaning and refresh
* Descriptive & inferential statistics (ANOVA, Regression)
* Pivot Tables with dynamic slicers and calculated fields
* Time-series forecasting (ETS and moving average)
* Executive summary chart design

#### Tableau Visualization

* Calculated fields and Level of Detail (LOD) expressions
* Multi-pane dashboards with linked filters and actions
* Interactive KPI and trend visuals
* Professional layout for executive audiences

#### Business Analytics Competencies

* Data-driven problem solving and ROI evaluation
* Hypothesis testing and decision modeling
* Storytelling with evidence-based insights
* Forecast-based strategic planning

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
      superstore_dashboard.twbx
      Dashboard with Tableau.png
    Executive-Presentation/
      insights_deck.pdf
    README.md
```


### Citation (APA 7th Edition)

Hirpa, S. T. (2025). *Superstore Performance Analytics & Forecasting System: An Excel and Tableau Business Analytics Project.* Arizona State University – Data Science with Business Analytics Track. Dataset source: Tableau Sample Superstore.

---
 **Next Steps:**

* Finalize Excel forecast sheet (ETS + Moving Average comparison).
* Update the dashboard with forecast trend and upload the public Tableau link.
* Commit changes to GitHub and reference this README in LinkedIn portfolio.

