# Quantium-Retail-Sales-Analytics
An end-to-end analysis of retail sales data, applying Python (Pandas, Matplotlib) to perform customer segmentation and evaluate an in-store trial's performance. Project by Quantium via Forage.

### Project Overview

This repository contains the complete data analysis for the Quantium Virtual Internship program by Forage. The project is an end-to-end analysis of retail sales data, focusing on customer purchasing behavior and the evaluation of an in-store trial to develop strategic recommendations for the chip category.

The analysis is broken down into three main tasks:
1.  **Customer Analytics:** Analyzing transaction and customer data to identify purchasing patterns and define key customer segments.
2.  **A/B Testing & Trial Evaluation:** Assessing the performance of a new store layout trial to determine its impact on sales and customer behavior.
3.  **Reporting & Strategic Recommendation:** Consolidating the findings into a clear, data-driven report for the Category Manager.

---

### 🛠️ Technologies & Libraries Used

*   **Python:** The primary language used for all data analysis.
*   **Pandas:** For data manipulation, cleaning, and transformation.
*   **Matplotlib & Seaborn:** For data visualization and creating insightful plots.
*   **Jupyter Notebook:** As the environment for interactive analysis and code development.
*   **SciPy:** For performing statistical analysis, specifically T-tests.

---

### 📂 Repository Structure

This repository is organized into the following sections:

*   **/data:** Contains the raw CSV datasets provided by Quantium.
    *   `QVI_transaction_data.xlsx`
    *   `QVI_purchase_behaviour.csv`
*   **/notebooks:** Contains the Jupyter Notebooks with the step-by-step analysis.
    *   `Task 1 - Customer Analytics.ipynb`: Data cleaning, feature engineering, and customer segmentation.
    *   `Task 2 - A/B Test Analysis.ipynb`: Control store selection, trial performance assessment, and statistical testing.
*   **/reports:** Contains the final presentation and key visuals.
    *   `Strategic Recommendations - Quantium.pptx`: The final PowerPoint presentation summarizing the findings for management.
*   `README.md`: This file, providing an overview of the project.

---

### 📈 Key Analyses & Findings

#### Task 1: Customer Analytics

*   **Data Cleaning & Preparation:** Processed and cleaned over 260,000 transaction records, handling outliers and creating new features like `brand` and `pack_size`.
*   **Customer Segmentation:** Identified three key customer segments based on purchasing behavior:
    1.  **Budget-Conscious:** Customers who prioritize value.
    2.  **Mainstream:** The largest customer group, representing a significant portion of sales.
    3.  **Premium:** High-spending customers who prefer premium brands.
*   **Key Insight:** Discovered that "Mainstream, Young Singles/Couples" are a primary driver of profitability, paying up to 10% more per unit due to their preference for premium chip brands.

#### Task 2: A/B Test Evaluation

*   **Control Store Selection:** Implemented a methodology to select suitable control stores by correlating and comparing pre-trial sales and customer data.
*   **Trial Performance Assessment:** Analyzed the performance of three trial stores against their selected control stores over a three-month period.
*   **Statistical Significance:** Conducted independent T-tests to determine if the observed sales uplift in the trial stores was statistically significant.
*   **Key Insight:** While two of the three trial stores showed a promising visual uplift in sales, the results were not statistically significant (p-value > 0.05), indicating that the increase could be due to random chance.

---

### 💡 Final Recommendation

Based on the analysis, the primary recommendation to the Category Manager was a two-pronged approach:

1.  **Target High-Value Segments:** Immediately implement targeted marketing promotions for "Mainstream, Young Singles/Couples" by strategically placing their preferred premium brands in high-traffic areas.
2.  **Extend the Trial:** Defer a decision on a national rollout of the new store layout. Extend the trial for another 3-4 months to gather more data, which will allow for a more statistically robust conclusion.

