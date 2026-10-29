# ApexPlanet Data Analytics Internship — Master Portfolio

**A 60-Day Data Analytics Internship | ApexPlanet Software Pvt. Ltd.**

This repository serves as the central overview of my ApexPlanet Data Analytics Internship, documenting my progression from data cleaning and exploratory analysis to business intelligence, statistical validation, and professional data storytelling.

Across four completed tasks, I applied Python, Pandas, SQL, Excel, Power BI, DAX, statistical hypothesis testing, and data visualization to analyze a retail sales dataset and communicate evidence-based findings.

**Internship project repository:** [ApexPlanet-Data-Analytics-Internship](https://github.com/Vijaygithubrit/ApexPlanet-Data-Analytics-Internship)

---

## Internship Progress

| Task | Project | Status |
|---|---|---|
| Task 1 | Data Immersion & Wrangling | Completed |
| Task 2 | Exploratory Data Analysis & SQL | Completed |
| Task 3 | Customer Segmentation & Interactive Dashboarding | Completed |
| Task 4 | Statistical Analysis & Data Storytelling | Completed |
| Task 5 | Capstone Integration & Portfolio Finalization | In Progress |

---

## Task 1 — Data Immersion & Wrangling

**Tools:** Python, Pandas, Jupyter Notebook, Excel

### Objective
Understand the dataset, identify data-quality issues, apply justified cleaning transformations, and prepare reliable data for analysis.

### Work completed
- Profiled the dataset's structure, columns, data types, and values.
- Investigated missing values, duplicate records, repeated identifiers, and outliers.
- Checked categorical consistency and numerical business rules.
- Converted order dates to an appropriate datetime format.
- Recovered missing values only where supporting evidence was available.
- Added a `Transaction_ID` to uniquely identify transaction records.
- Validated the cleaned dataset and documented decisions.

### Key learnings
- Data quality must be assessed before drawing business conclusions.
- Missing values should not be filled using unsupported assumptions.
- Repeated order identifiers do not automatically mean duplicate transactions.
- Validation rules help detect inconsistent or invalid records.
- Data-cleaning decisions should be transparent and reproducible.

**Deliverables:** Cleaning notebook, data dictionary, raw and cleaned datasets, profiling outputs, and validation documentation.

**[Explore Task 1 in the internship repository](https://github.com/Vijaygithubrit/ApexPlanet-Data-Analytics-Internship/tree/main/01_Task_1_Data_Wrangling)**

---

## Task 2 — Exploratory Data Analysis & SQL

**Tools:** Python, Pandas, NumPy, MySQL, SQL, Matplotlib, Jupyter Notebook

### Objective
Explore sales performance, investigate customer and product patterns, and answer business questions through Python analysis, SQL queries, and visualizations.

### Work completed
- Performed descriptive statistics and exploratory data analysis.
- Investigated monthly sales, product categories, products, cities, and customer characteristics.
- Created SQL aggregations, filtering, grouping, ranking, and customer-level queries.
- Generated visualizations for sales trends, category and product comparisons, city performance, and correlations.
- Built a retail sales dashboard.
- Documented data-quality issues, findings, and analytical limitations.

### Key learnings
- EDA helps identify patterns, anomalies, and questions that need further investigation.
- SQL is effective for aggregating data and answering structured business questions.
- Visualizations make complex results easier to interpret.
- Correlation describes association, not causation.
- Incomplete periods and inconsistent customer identifiers can affect conclusions.

### Selected findings
- Recorded total sales: approximately 139.40 million in the dataset's numerical units.
- Leading category by sales: Electronics.
- Leading product by sales: Laptop.
- Peak recorded sales month: March 2025.

These results describe the supplied dataset. The currency and business context should be verified before interpreting the values as a specific monetary amount.

**Deliverables:** EDA notebook, SQL queries, dashboard, charts, findings report, and supporting analysis.

**[Explore Task 2 in the internship repository](https://github.com/Vijaygithubrit/ApexPlanet-Data-Analytics-Internship/tree/main/02_Task_2_EDA_SQL)**

---

## Task 3 — Customer Segmentation & Interactive Dashboarding

**Tools:** Microsoft Power BI, DAX, Power Query, Excel, data modeling and visualization

### Objective
Analyze customer purchasing behavior, create customer segments, develop business KPIs, and communicate sales performance through an interactive Power BI dashboard.

### Work completed
- Built a customer-level summary table.
- Calculated customer sales, order counts, quantities, and purchase metrics.
- Created KPI measures for total sales, customers, orders, average order value, and sales per customer.
- Ranked customers and segmented them using sales percentiles.
- Built customer segment, category contribution, and monthly sales visualizations.
- Added interactive filters and improved dashboard layout and formatting.

### Customer segments
- **High-Value:** Customer sales at or above the 80th percentile.
- **Regular:** Customer sales at or above the 40th percentile but below the 80th percentile.
- **Occasional:** Customer sales below the 40th percentile.

### Key learnings
- Data modeling and DAX support reusable, interactive business metrics.
- Customer segmentation turns transaction-level data into actionable customer groups.
- KPI definitions must be clear and consistent with the underlying data.
- Slicers and filters help stakeholders investigate specific periods and categories.
- Partial reporting periods can distort monthly comparisons.
- Sales-based segments do not automatically measure profitability or customer lifetime value.

**Deliverables:** Interactive Power BI dashboard, `.pbix` file, dashboard screenshot, and deep-dive analysis report.

**[Explore Task 3 in the internship repository](https://github.com/Vijaygithubrit/ApexPlanet-Data-Analytics-Internship/tree/main/03_Task_3_Deep_Dive_Dashboard)**

---

## Task 4 — Statistical Analysis & Data Storytelling

**Tools:** Python, Pandas, NumPy, SciPy, Matplotlib, PowerPoint

### Objective
Investigate data-quality concerns, test whether observed differences between customer groups are statistically significant, and communicate the results responsibly.

### Work completed
- Investigated repeated order identifiers and inconsistent customer attributes.
- Prepared customer-level summary data.
- Formulated null and alternative hypotheses.
- Conducted a two-sided Welch independent-samples t-test.
- Calculated the p-value and 95% confidence interval.
- Performed sensitivity analysis after temporarily excluding records associated with a flagged order identifier.
- Prepared a written analysis report and PowerPoint presentation.

### Primary statistical results

| Metric | Result |
|---|---:|
| Male customers included | 468 |
| Female customers included | 445 |
| Difference in sample means (male − female) | 5,766.91 |
| Welch's t-statistic | 0.7728 |
| p-value | 0.439854 |
| 95% confidence interval | −8,878.91 to 20,412.73 |
| Decision at α = 0.05 | Fail to reject the null hypothesis |

### Interpretation
The observed difference was not statistically significant at the 5% level. The confidence interval includes zero, so the analysis did not establish a statistically significant difference between the population means.

This does **not** prove that the groups are equal. The measure is customer-level average recorded transaction sales, and the dataset's currency and business definitions have not been independently verified.

### Key learnings
- Hypothesis testing provides a structured way to evaluate observed differences.
- A p-value is not the probability that the null hypothesis is true.
- Confidence intervals communicate the uncertainty around an estimated difference.
- A non-significant result does not establish equality.
- Sensitivity analysis tests whether conclusions change under alternative data-handling decisions.
- Statistical findings should be communicated with assumptions, limitations, and appropriate business context.

**Deliverables:** Analysis scripts, CSV outputs, hypothesis-test results, visualization, deep-dive report, PowerPoint presentation, and presentation video.

**[Explore Task 4 in the internship repository](https://github.com/Vijaygithubrit/ApexPlanet-Data-Analytics-Internship/tree/main/04_Task_4_Statistics_Storytelling)**

**[View the Task 4 PowerPoint presentation](https://github.com/Vijaygithubrit/ApexPlanet-Data-Analytics-Internship/blob/main/04_Task_4_Statistics_Storytelling/ppt/ApexPlanet_Task4_Statistical_Storytelling.pptx)**

---

## Task 5 — Capstone Integration & Portfolio Finalization

**Status:** In Progress

### Objective
Bring the completed internship work together into a clear, professional master repository that demonstrates the complete analytics workflow, technical skills, deliverables, and key learnings.

### Progress completed
- Reviewed documentation for Tasks 1–4.
- Created a separate portfolio website prototype using HTML, CSS, and JavaScript.
- Uploaded the prototype to a dedicated GitHub repository.
- Successfully deployed the prototype through GitHub Pages.

### Remaining work
- Complete the final review of all task links and deliverables.
- Ensure the master documentation is consistent and accurate.
- Finalize the internship presentation and professional reflection.
- Prepare a LinkedIn post summarizing the internship and linking to this master repository.
- Update the status when all required Task 5 deliverables are finished.

### Prototype links
- [Separate portfolio prototype repository](https://github.com/Vijaygithubrit/Vijay-Data-Analyst-Portfolio)
- [Open the deployed prototype](https://vijaygithubrit.github.io/Vijay-Data-Analyst-Portfolio/)

**Note:** This prototype is separate from my future main personal portfolio website.

---

## Technical Skills Demonstrated

| Area | Skills |
|---|---|
| Programming | Python, Pandas, NumPy |
| Data preparation | Data cleaning, missing-value analysis, validation, data profiling |
| Databases | MySQL, SQL aggregations, filtering, grouping, ranking |
| Business intelligence | Power BI, DAX, KPIs, customer segmentation |
| Visualization | Matplotlib, dashboard design, sales trend analysis |
| Statistics | Descriptive statistics, Welch's t-test, p-values, confidence intervals, sensitivity analysis |
| Communication | Analytical reports, PowerPoint, data storytelling |
| Development | Git, GitHub, Markdown, HTML, CSS, JavaScript, GitHub Pages |

---

## End-to-End Analytics Workflow

**Data preparation → Exploratory analysis → SQL business analysis → Customer segmentation → Statistical validation → Reporting and storytelling**

This progression demonstrates how analytical work moves from assessing data quality to exploring patterns, building business metrics, testing claims, and communicating results with appropriate context.

---

## Professional Reflection

This internship strengthened my ability to work through an end-to-end data analytics process rather than relying on a single tool or visualization.

The most important lessons were to validate data before analyzing it, define business metrics carefully, distinguish correlation from causation, interpret statistical results responsibly, and communicate findings with transparent limitations.

Going forward, I aim to apply these skills to practical business problems and continue developing my capabilities in SQL, Python, Power BI, statistics, and analytical communication.

---

## Main Project Repository

**[ApexPlanet Data Analytics Internship — Tasks 1–4 and supporting deliverables](https://github.com/Vijaygithubrit/ApexPlanet-Data-Analytics-Internship)**

**[GitHub Profile](https://github.com/Vijaygithubrit)**

*Task 5 remains in progress until the remaining internship documentation and final deliverables are completed.* 🚀
