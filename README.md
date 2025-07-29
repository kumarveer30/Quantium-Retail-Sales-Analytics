# Quantium - Retail Strategy and Analytics for Chip Sales

### **Project Overview**
This repository documents an end-to-end data analysis project conducted for a supermarket client to enhance their chip category strategy. The project involves analyzing 12 months of transaction and customer data to understand purchasing behavior, identify key customer segments, and measure the impact of a new store layout trial. The entire analysis was performed using Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy).

---

### **1. Business Problem**

The Category Manager for Chips at a major supermarket chain needs to develop a strategic plan for the upcoming year. To do this, they require a deep understanding of who their customers are and how they purchase chips. The core business problems are:

*   **Lack of Customer Understanding:** The client has a rich dataset but lacks a clear understanding of which customer segments are most valuable and what drives their purchasing behavior.
*   **Need for Actionable Insights:** The client needs data-driven recommendations to identify opportunities for growth in the chip category.
*   **Measuring In-Store Trial Impact:** The client performed a trial of a new store layout in three stores (77, 86, and 88) and needs to know if the changes led to a significant increase in sales. This requires a robust analytical approach to measure the sales uplift against comparable control stores.

As part of Quantium's retail analytics team, my task was to analyze the provided data and deliver a strategic recommendation to the Category Manager.

---

### **2. Project Goal**

The primary goal of this analysis is to provide the Category Manager with a data-supported strategic recommendation for the upcoming category review. This was achieved through two main phases:

*   **Phase 1: Customer Analytics:**
    *   Perform a deep-dive analysis of customer segments to identify which groups are most valuable to the chip category.
    *   Define the key metrics that describe customer purchasing behavior (e.g., spend, frequency, units per transaction).
    *   Deliver initial findings on sales drivers and interesting trends to inform the overall strategy.

*   **Phase 2: Trial Store Evaluation:**
    *   Develop a data-driven methodology to select suitable control stores that are statistically comparable to the three trial stores.
    *   Assess the performance of the trial stores during the trial period by comparing their sales uplift against the control stores.
    *   Determine if the trial was successful and provide a final recommendation on a potential national rollout of the new store layout.

---

### **3. Key Analyses & Visualizations**

The analysis was conducted in a Jupyter Notebook, with key findings visualized to support the final recommendations.

#### **Customer Segment Analysis**
*   **Total Sales by Lifestage & Premium Status (Bar Chart):**
    *   **Description:** This visual breaks down total chip sales by the two key customer dimensions: `LIFESTAGE` (e.g., "Young Singles/Couples", "Families") and `PREMIUM_CUSTOMER` (e.g., "Budget", "Mainstream", "Premium").
    *   **Purpose:** To identify the highest-value customer segments at a glance. This chart immediately highlights which groups contribute the most to revenue.

*   **Units per Customer by Segment (Bar Chart):**
    *   **Description:** This chart shows the average number of chip packets purchased per customer within each segment.
    *   **Purpose:** To understand the purchasing volume of different segments, helping to differentiate between high-frequency and high-quantity shoppers.

*   **Average Price per Unit by Segment (Bar Chart):**
    *   **Description:** This visual displays the average price customers are willing to pay per unit of chips, segmented by lifestage and premium status.
    *   **Purpose:** To identify which customer segments are less price-sensitive and are willing to pay more for premium or larger-sized products. This is a key indicator of profitability.

#### **A/B Test & Trial Store Analysis**
*   **Control Store Selection (Correlation Heatmap & Line Charts):**
    *   **Description:** To find the best control store for each trial store, a correlation analysis was run on monthly sales and customer counts for all non-trial stores. The store with the highest correlation was chosen. This was visualized with line charts comparing the pre-trial sales trends of the trial store and its selected control store.
    *   **Purpose:** To establish a credible baseline for comparison, ensuring that the control store's performance is a reliable proxy for what the trial store would have achieved without the new layout.

*   **Trial Performance Assessment (Line Chart & Bar Chart):**
    *   **Description:** For each trial/control pair, a line chart plots their total monthly sales over the full year, with the trial period highlighted. A separate bar chart shows the percentage uplift in sales for the trial store during the trial period.
    *   **Purpose:** To visually and quantitatively assess the impact of the new layout. The line chart shows the trend divergence, while the bar chart provides a clear measure of the sales uplift.

*   **Statistical Significance Test (T-Test):**
    *   **Description:** A two-sample t-test was performed on the sales data from the trial and control stores during the trial period. The resulting p-value was used to determine if the observed sales uplift was statistically significant.
    *   **Purpose:** To provide mathematical rigor to the findings and confirm that the sales increase was due to the new layout and not just random chance.

---

### **4. Business Impact & Insights**

The analysis yielded several commercially significant insights that directly informed the client's strategy:

*   **Insight 1: Identified Key Customer Segments:** The analysis revealed that **"Mainstream - Young Singles/Couples"** and **"Mainstream - Retirees"** were critical segments. While not the highest spenders overall, they purchase chips more frequently and are more willing to pay a higher price per unit, making them a highly profitable target audience.

*   **Insight 2: Recommended Targeting Strategy:** Based on the segment analysis, the recommendation was to focus marketing efforts on the "Mainstream - Young Singles/Couples" segment. Their higher propensity to purchase larger, more expensive chip packets presents a clear opportunity to drive incremental revenue.

*   **Insight 3: Successful Trial in Two Stores:** The A/B testing analysis showed a **statistically significant sales uplift** in trial stores 77 and 88 compared to their control stores. This provided a data-backed validation that the new store layout was effective in these locations.

*   **Insight 4: Actionable Rollout Recommendation:** For trial store 86, the sales uplift was not statistically significant, suggesting the new layout was not as effective there. The final recommendation was to **roll out the new layout to stores similar to 77 and 88**, while further investigating the performance drivers in store 86 before making a broader decision. This nuanced recommendation helped the client avoid a costly, one-size-fits-all national rollout.

