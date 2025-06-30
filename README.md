# crime_against_on_womensIn this notebook, we perform an in-depth exploratory and descriptive analysis of the **Crimes Against Women** dataset, which contains reported cases across Indian states and union territories from the years 2001 to 2021. This dataset provides critical insights into the frequency, types, and distribution of crimes committed against women, making it a valuable resource for policy formulation, social awareness, and data-driven intervention planning.

The purpose of this analysis is to uncover patterns, identify high-risk regions, examine the most prevalent types of crimes, and understand long-term trends in gender-based violence. We place particular emphasis on visualizing changes over time, comparing crime volumes across different states, and assessing the impact of specific types of violence such as **domestic abuse**, **assault on modesty**, **rape**, and **trafficking**.

By analyzing the cleaned and reshaped dataset, we aim to build a strong foundation for more advanced statistical or predictive modeling and inform future policy recommendations or public safety initiatives.

---

We begin our analysis by importing essential Python libraries used for **data manipulation**, **visualization**, and **file handling**:

- `pandas`: Used for loading, cleaning, and reshaping structured tabular data, allowing efficient data analysis workflows.

- `numpy`: Supports numerical operations and handling of missing or inconsistent data values.

- `os`: Helps manage file paths and directories during the analysis and export process.

- `plotly.express`: A powerful graphing library used to create interactive and insightful visualizations that reveal key patterns and trends across states, years, and crime categories.
  Statistical Testing and Correlation Analysis

In this section, we apply two key statistical methods to the crime dataset:

1. **Chi-Square Test of Independence**  
   A contingency table is created using `State` and `Crime Type` to examine whether there is a statistically significant association between the state where a crime occurred and the type of crime reported.

   - A **low p-value (< 0.05)** indicates a **significant relationship** between state and crime type, suggesting some crimes are more common in certain states.

2. **Spearman Correlation Analysis**  
   For each crime type, the correlation between **year** and **number of reported cases** is measured using Spearman's rank correlation.
   - This helps identify whether a specific crime type is **increasing or decreasing** over time.
   - Significant correlations guide understanding of **long-term crime trends**.

The results provide statistical backing for visual trends observed earlier and offer direction for targeted interventions or future modeling.
