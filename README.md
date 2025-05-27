# 📊 AdventureWorks Industry Procurement Analysis - Power BI
<p align="center">
  <img src="https://github.com/user-attachments/assets/23b1ad67-fc1d-4124-8efe-d04eb1acdcf6" alt="AdventureWorks Project Banner" width="1000"> 
</p>

* **Author:** Nguyen Thi Thuy Dung
* **Date:** 2025-04
* **Tools Used:** Microsoft Power BI, DAX, Excel (for Design Thinking), SQL (SQL Server)

---

## 📑 Table of Contents
- [📌 Background & Overview](#-background--overview)
- [📂 Project Focus & Dataset Context](#-project-focus--dataset-context)
- [🧠 Design Thinking Process](#-design-thinking-process)
- [⚒️ Main Process: Data Preparation & Dashboard Development](#%EF%B8%8F-main-process-data-preparation--dashboard-development) 
- [📊 Key Insights & Visualizations](#-key-insights--visualizations)
- [🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)
- [🚀 Usage Instructions](#-usage-instructions) 
- [📂 Project Deliverables](#-project-deliverables)
- [💡 Design Discussions and Decisions](#design-discussions-and-decisions) 

---

## 📌 Background & Overview

### Objective
📖 **What is this project about?**

This project analyzes **AdventureWorks' procurement operations** to support strategic decision-making in the **manufacturing industry**. By visualizing purchasing data, the dashboard helps improve efficiency, control costs, and monitor vendor performance.

It aims to:
*   ✔️ Highlight trends in **purchasing costs**, **order volumes**, and **fulfillment time**.
*   ✔️ Assess **operational efficiency** via unit prices, lead times, and vendor activities.
*   ✔️ Evaluate the **performance** and **cost-effectiveness of shipping methods**.

👤 **Who is this project for?**
*   AdventureWorks Leadership & Management
*   Procurement Department Managers & Staff
*   Data Analysts & Business Analysts supporting procurement.

🎯 **Project Outcome:**
*   **Cost & Volume Insights:** Successfully identified seasonal ordering patterns and pinpointed "Components" as a primary cost driver.
*   **Operational Efficiency Gains:** Highlighted opportunities for lead time reduction and more effective shipping method analysis.
*   **Strategic Foundation:** Provided a data-backed basis for optimizing procurement strategies, including supplier evaluation and cost management for key materials.

---

## 📌 Project Focus & Dataset Context

This project focuses on analyzing the **Production and Procurement processes** within a manufacturing context. This is achieved by modeling and visualizing data sourced from the **AdventureWorks database**.

### 🧱 Data Structure

The analysis utilizes a total of **12 tables** from the AdventureWorks database, structured as follows:

*   **Dimension Tables (5):**
    *   `Product_Product`
    *   `Product_ProductTable`
    *   `Production_Location`
    *   `Production_ScrapReason`
    *   `Purchasing_Vendor`

*   **Fact Tables (7):**
    *   `Product_Inventory`
    *   `Production_BillOfMaterials`
    *   `Production_WorkOrder`
    *   `Production_WorkOrderRouting`
    *   `Purchasing_OrderDetail`
    *   `Purchasing_OrderHeader`
    *   `Purchasing_ProductVendor`

---

## 🧠 Design Thinking Process
This project applied **Design Thinking principles** to thoroughly understand leadership's needs regarding procurement insights and to define the dashboard's scope effectively. 

1️⃣ **Empathize:** Focused on understanding the daily challenges and strategic objectives of the Procurement Department and AdventureWorks leadership.
<p align="center">
  <img src="https://github.com/user-attachments/assets/edd92688-1279-4453-be25-43b69a79729c" alt="Design Thinking: Empathize Stage - Understanding User" width="900">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/5c7c4dc4-5a41-4c3c-a3ee-7f8b7bf2ec0f" alt="Design Thinking: Empathize Stage - Stakeholder Map" width="700">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/787125b9-8617-45c4-b872-27dc15fd9759" alt="Design Thinking: Empathize Stage - Journey Map" width="500">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/f0ba90fa-9acb-4038-9300-52aaaa016509" alt="Design Thinking: Empathize Stage - Journey Map" width="950">
</p>

2️⃣ **Define (Point of View):** Articulated the core problem: The necessity for a clear, consolidated, and data-driven overview of all procurement activities to enable informed and timely decision-making.
<p align="center">
  <img src="https://github.com/user-attachments/assets/e7e46fc3-fe62-4724-a8ed-eb9214b2a92a" alt="Design Thinking: Define Stage - POV" width="600">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/d0088948-9a6d-4d0d-a653-6d6db59fa379" alt="Design Thinking: Define Stage - HMW Questions" width="600">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/ea9ddf9f-7ba2-458a-aaaa-fb8a8420a007" alt="Design Thinking: Define Stage - User Needs" width="700">
</p>

3️⃣ **Ideate:** Brainstormed a range of relevant Key Performance Indicators (KPIs), effective data visualizations, and intuitive dashboard layouts designed to directly address the defined problem statement and business questions.
<p align="center">
  <img src="https://github.com/user-attachments/assets/005deca6-fe55-4bdc-a38f-e98642e7469c" alt="Design Thinking: Ideate Stage - Brainstorming" width="700">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/18fbaa14-7502-44d8-9a2f-02bfaa644070" alt="Design Thinking: Ideate Stage - Prioritization" width="500">
</p>

4️⃣ **Prototype and Review:** Developed initial dashboard prototypes in Power BI, which were then iteratively refined based on analytical goals, data storytelling principles, and assumed stakeholder feedback for maximum clarity and impact.
<p align="center">
  <img src="https://github.com/user-attachments/assets/25bea8f6-5e83-48e2-9132-a53dac0ab6b2" alt="Design Thinking: Prototype Stage - Dashboard Sketch" width="900">
</p>

---

## ⚒️ Main Process: Data Preparation & Dashboard Development

### 1️⃣ Data Preparation (Power Query & DAX)
*   Connected to the **AdventureWorks SQL Server database** within Power BI.
*   Selected and imported tables and columns pertinent to the **Purchasing** analysis.
*   Performed necessary data type transformations and handled missing values using **Power Query Editor**.
*   Created essential calculated columns and **DAX measures** for key procurement metrics (e.g., `Total Purchase Cost (YTD)`, `Average Lead Time Overall`).

### 2️⃣ Power BI Visualization & Dashboarding
Developed interactive and insightful dashboards tailored to specific stakeholder needs, focusing on clear data presentation and actionable insights.

---

## 📊 Key Insights & Visualizations

🔍 **Dashboard Previews & Analysis**

The procurement operations dashboard is structured into user-centric pages:

### **Page 1: Purchasing Overview - Cost & Volume**
<p align="center">
  <img src="https://github.com/user-attachments/assets/2638998c-0819-4ac1-aa66-1c1fe8ed32d0" alt="Purchasing Overview: Cost & Volume Dashboard" width="900">
</p>

📌 **Analysis (Cost & Volume):**
* **Key Discoveries:**

1.  **Historical Operational Scale:**
    *   The total historical purchase cost amounts to **$70.48 million**, with an average purchase order value of **$17.57 thousand**. This indicates significant investment and a tendency towards high-value procurement transactions.

2.  **Strategic Product "ProductID 528":**
    *   A specific product, **ProductID 528**, is closely monitored, with a total of **50 distinct orders** placed for it (each order being a conventional "package" with `OrderQty = 3`, resulting in a `Sum of OrderQty Values` of 150) throughout the data's history. This highlights the importance or unique ordering process of this product.

3.  **Spending Structure for Top 5 Vendors:**
    *   A detailed analysis of the Top 5 vendors (based on total purchase cost) shows this group contributes significantly to overall spending. The total purchase cost from these **Top 5 vendors amounts to $17.36 million** across the recorded years.
    *   This figure represents approximately **24.6%** ($17.36M / $70.48M) of the total historical purchase cost, indicating a notable concentration on top-tier supply partners.
    *   In the detailed data displayed, **"Chicago City Saddles"** is a prominent vendor appearing within this group.

4.  **Pronounced Seasonal Trends (Aggregated Across Years):**
    *   Procurement activities exhibit strong seasonality. Costs typically rise from the beginning of the year, **peaking in June** (with a total expenditure of $8.08M across all Junes).
    *   Subsequently, costs tend to decrease significantly towards the end of Q3 (September and October being the lowest).
    *   Orders for `ProductID` 528 (potentially supplied by one or more of the Top 5 vendors) also follow a similar seasonal pattern.

5.  **Key Cost Drivers:**
    *   Monthly cost fluctuations are primarily driven by **changes in order volume**.
    *   However, there are positive indications that "price" (encompassing base price, taxes, and fees) tends to decrease or have a cost-reducing impact in the later months of the year, suggesting cost optimization capabilities.

**Overall Narrative:** This dashboard tells a compelling story of a business with large-scale procurement operations that follow clear seasonal cycles. A quarter of the spending is concentrated within the Top 5 vendor group, with "Chicago City Saddles" being a notably detailed name. Furthermore, the close monitoring of the strategic product "ProductID 528" (which may be linked to these top vendors) indicates a focus on core elements.


### **Page 2: Purchasing Operations - Efficiency, Details & Vendor Insights**
<p align="center">
  <img src="https://github.com/user-attachments/assets/5a9319a0-00b4-42c9-b0aa-0e1dbfb611d9" alt="Purchasing Operations: Efficiency & Details Dashboard" width="900">
</p>

📌 **Analysis (Operational Efficiency & Delivery):**
*   **Key Discoveries:**

1.  **Stability of Core Products & Lead Times:**
    *   **Average Unit Price: 38.16** for the tracked "conventional units" (most likely related to `ProductID` 528), indicating consistent pricing from suppliers.
    *   **Average Lead Time Overall: 19.45 days**. This is the standard time from order placement to receipt, a crucial KPI for planning.
    *   **Active Vendors YTD: 86 vendors** in 2014 (the most recent year with data), showcasing a diversified supply base.

2.  **Preferred Shipping Methods:**
    *   The business predominantly relies on **Ship Method IDs 5 (1523 orders) and 4 (1085 orders)**, accounting for the majority of the approximately 4012 historical orders. This suggests optimization in selecting transport channels.

3.  **Ancillary Cost Structure (Freight & Tax):**
    *   **Freight costs constitute about 2.48% and taxes about 8.00%** of the total SubTotal value.
    *   These rates exhibit **remarkable stability across months**, making procurement cost forecasting more accurate.

4.  **Monthly Order Value Fluctuation & Processing Efficiency (Aggregated Across Years):**
    *   *Average Order Value:* While order volumes might decrease in certain months, **October stands out with a significantly high average order value (over $20K)**, suggesting strategic purchases or high-value item procurement.
    *   *Average Order Processing Time:* Internal processing is quite stable, **averaging around 9 days**. However, a **slight increase to 9.22 days in November** warrants attention, possibly due to year-end workload increases.
  
**Overall Narrative:**
This page reveals **stability and control** in detailed operations: from consistent core product unit prices and preferred shipping channels to maintained ancillary cost rates. Concurrently, it highlights points of attention such as **high-value orders concentrating in October** and a slight **fluctuation in year-end order processing efficiency**, opening avenues for further optimization.

---

## 🔎 Final Conclusion & Recommendations
👉🏻 Based on the comprehensive analysis facilitated by the Power BI dashboards, the AdventureWorks Purchasing Department and Leadership should consider the following strategic actions for enhanced operational control and cost-efficiency:

📌 **Key Takeaways:**
*   ✔️ **Embrace Seasonal Planning:** Proactively manage inventory and supplier orders in alignment with identified seasonal purchasing trends to optimize costs and ensure material availability.
*   ✔️ **Targeted Cost Optimization:** Concentrate cost-reduction efforts on high-spend categories, particularly "Components," through avenues like supplier negotiation or exploring alternative sourcing.
*   ✔️ **Prioritize Lead Time Reduction:** Implement process improvements and collaborate with suppliers to significantly shorten the overall order fulfillment cycle, thereby improving responsiveness.
*   ✔️ **Strategic Shipping Method Evaluation:** Continuously assess and select shipping methods to ensure an optimal balance of logistical cost and delivery speed.
*   ✔️ **Enhance Vendor Performance Monitoring:** Develop and implement a robust system for tracking and evaluating vendor performance against key metrics such as on-time delivery, price stability, and quality.

---

## 🚀 Usage Instructions
*   Open the `.pbix` file using **Microsoft Power BI Desktop**.
*   Interact with the dashboard using **Slicers** (e.g., for `Date`, `Product Category`) and **cross-filtering** capabilities by clicking on visual elements.
*   Hover over visuals to view detailed **tooltips**.

---

## 📂 Project Deliverables
1.  **Power BI Dashboard (`.pbix` file):** [View Dashboard](https://github.com/Dung040125/AdventureWorks---Procurement-Operations-Dashboard-Power-BI-/raw/main/Project3_DataSourceImported.pbix)
2.  **Design Thinking Excel File:** Documents the user-centric design process and detailed findings. [View file](https://github.com/Dung040125/AdventureWorks---Procurement-Operations-Dashboard-Power-BI-/raw/main/Design%20Thinking%20_%20project%203.xlsx)

---

## 💡Design Discussions and Decisions
Key design choices and interpretations made during this project include:
*   **Focus on Core Procurement KPIs:** Prioritized metrics directly impacting **cost, timeliness, and efficiency** relevant to the Purchasing Department's objectives.
*   **Stakeholder-Centric Dashboard Design:** Dashboards were conceptualized to serve typical leadership needs for **high-level overviews and actionable operational insights**.
*   **Data Scope for Purchasing:** Selected a relevant subset of AdventureWorks tables pertinent to the **Purchasing** topic to maintain focus and deliver actionable results.
*   **Iterative Refinement:** The development of visualizations and insights was an iterative process, continuously refining views to best address core business questions.

*(Further details on specific data transformations, DAX measures, and visualization choices are implicitly covered in the dashboard design and can be further explored in the Design Thinking artifacts.)*
