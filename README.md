# AdventureWorks-Procurement-Operations-Dashboard-PowerBI-
Power BI operations dashboard analyzing AdventureWorks Cycles' procurement data to provide actionable insights for leadership on purchasing costs, operational efficiency, and vendor management.

---
## Summary
This project presents an Operations Dashboard built with Power BI, analyzing the procurement data of AdventureWorks Cycles. The dashboard provides leadership with a visual and understandable overview of purchasing activities, supporting decision-making and operational optimization, focusing on costs, order efficiency, and delivery details.

---
## Table of Contents
- [Introduction & Objectives](#introduction--objectives)
- [Dataset & Preprocessing](#dataset--preprocessing)
- [Methodology & Tools](#methodology--tools)
- [Dashboard Overview & Key Pages](#dashboard-overview--key-pages)
    - [Purchasing Overview: Cost & Volume](#purchasing-overview-cost--volume)
    - [Purchasing Operations: Efficiency, Details & Vendor Insights](#purchasing-operations-efficiency-details--vendor-insights)
- [Key Insights & Recommendations](#key-insights--recommendations)
- [Usage Instructions](#usage-instructions)
- [Project Deliverables](#project-deliverables)

---
## Introduction & Objectives
The Purchasing Department of AdventureWorks Cycles needs to ensure an efficient supply chain (sufficient stock, on-time delivery, optimal pricing). This project develops an Operations Dashboard using Power BI to:
*   Provide a comprehensive overview of purchasing costs, quantities, and trends.
*   Analyze operational efficiency, delivery details, and vendor-related factors.
*   Support data-driven decision-making by leadership to improve procurement processes.

---
## Dataset & Preprocessing
-   **Dataset:** AdventureWorks Database, focusing on **Purchasing** data.
-   **Preprocessing (Power Query):**
    -   Connected, cleaned, and transformed data from the AdventureWorks source.
    -   Built a data model, established relationships, and created DAX measures (`Total Purchase Cost (YTD)`, `Avg Lead Time Overall`, etc).

---
## Methodology & Tools
-   **Process:**
    -   Applied Design Thinking (Excel) to identify leadership's needs.
    -   Analyzed requirements, preprocessed data, built the data model, and developed DAX measures.
    -   Designed the dashboard in Power BI, summarizing insights and recommendations.
-   **Tools:** Microsoft Power BI Desktop, Microsoft Excel.
-   **Language:** DAX.

---
## Dashboard Overview & Key Pages
The dashboard comprises specialized pages for analyzing procurement activities:

### Purchasing Overview: Cost & Volume
Provides an overview of purchasing costs, order quantities over time, and cost structure by category.
*   **Key Visuals:** KPIs (`Total Purchase Cost YTD`, `Total Quantity Ordered MTD`), `Monthly Quantity and Orders`, `Monthly Cost Trend`, `Cost Impact Analysis`, `Category Cost Share`.
![image](https://github.com/user-attachments/assets/81ac067f-0ad7-497f-84fc-950611f675fd)


### Purchasing Operations: Efficiency, Details & Vendor Insights
Analyzes operational efficiency, shipping costs, taxes, order fulfillment times, and factors related to vendor performance.
*   **Key Visuals:** KPIs (`Avg Unit Price`, `Avg Lead Time Overall`, `Active Vendors YTD`), `Order Count by Ship Method ID`, `Monthly Orders & Avg Value`, `Monthly Freight & Tax Analysis`, `Overall Order Fulfillment Time Trend`.
*(This page also implicitly covers or can be extended for a more detailed analysis of vendor performance and associated costs.)*
![image](https://github.com/user-attachments/assets/32ff243f-1e3a-41f4-a900-f190b3c50d11)

---
## Key Insights & Recommendations
![image](https://github.com/user-attachments/assets/7c0678a9-e2bb-4558-8161-77c6fc1b0ad2)


Based on the analysis (details in the image above and the Design Thinking file):

**Regarding Cost & Volume:**
*   **Insight:** Ordering activity and costs tend to decrease in Q3-early Q4, recovering by year-end. "Components" account for a large share of costs.
*   **Recommendation:** Optimize costs for "Components." Plan for seasonal trends (Q3/Q4). Control prices during months with high "Cost Impact by Price."

**Regarding Operational Efficiency & Delivery Details:**
*   **Insight:** Need to shorten order-to-ship times. A thorough analysis of cost/speed for each shipping method ID is necessary. Average order value significantly drops in October.
*   **Recommendation:** Optimize Lead Time. Evaluate and optimize shipping methods. Review order sizes (especially in months with low average value). Closely monitor Freight & Tax costs.

---
## Usage Instructions
-   Open the `.pbix` file using Microsoft Power BI Desktop.
-   Interact with the dashboard via Slicers (`Date`, `Category`, `Year`) and cross-filtering. Hover over visuals for tooltips.

---
## Project Deliverables
1.  **Power BI Dashboard (`.pbix` file):** [View Dashboard](https://github.com/Dung040125/AdventureWorks---Procurement-Operations-Dashboard-Power-BI-/raw/main/Project3_DataSourceImported.pbix)
2.  **Design Thinking Excel File:** Documents the design process, analysis, and detailed recommendations. [View file](https://github.com/Dung040125/AdventureWorks---Procurement-Operations-Dashboard-Power-BI-/raw/main/Design%20Thinking%20_%20project%203.xlsx)

