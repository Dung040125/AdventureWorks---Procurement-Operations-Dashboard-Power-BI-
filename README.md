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
  <img src="https://github.com/user-attachments/assets/0ef2a795-ace9-441f-9ec5-acf860776dc1" alt="Design Thinking: Empathize Stage - Understanding User" width="700">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/0e8afd7b-de6d-4eb4-8604-cd7625eb6b0f" alt="Design Thinking: Empathize Stage - Stakeholder Map" width="700">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/e86854e1-642d-4c06-ae83-9de6b791097d" alt="Design Thinking: Empathize Stage - Journey Map" width="700">
</p>

2️⃣ **Define (Point of View):** Articulated the core problem: The necessity for a clear, consolidated, and data-driven overview of all procurement activities to enable informed and timely decision-making.
<p align="center">
  <img src="https://github.com/user-attachments/assets/590ca0ec-d9ba-4f33-bff1-9617cb0342f2" alt="Design Thinking: Define Stage - POV" width="700">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/d0088948-9a6d-4d0d-a653-6d6db59fa379" alt="Design Thinking: Define Stage - HMW Questions" width="700">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/71a855c9-e7d0-4592-b926-e280a981c287" alt="Design Thinking: Define Stage - User Needs" width="700">
</p>

3️⃣ **Ideate:** Brainstormed a range of relevant Key Performance Indicators (KPIs), effective data visualizations, and intuitive dashboard layouts designed to directly address the defined problem statement and business questions.
<p align="center">
  <img src="https://github.com/user-attachments/assets/005deca6-fe55-4bdc-a38f-e98642e7469c" alt="Design Thinking: Ideate Stage - Brainstorming" width="700">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/f27bdc4a-fde7-4384-9e25-a8c648ef38b4" alt="Design Thinking: Ideate Stage - Prioritization" width="700">
</p>

4️⃣ **Prototype and Review:** Developed initial dashboard prototypes in Power BI, which were then iteratively refined based on analytical goals, data storytelling principles, and assumed stakeholder feedback for maximum clarity and impact.
<p align="center">
  <img src="https://github.com/user-attachments/assets/25bea8f6-5e83-48e2-9132-a53dac0ab6b2" alt="Design Thinking: Prototype Stage - Dashboard Sketch" width="700">
</p>

---

## ⚒️ Main Process: Data Preparation & Dashboard Development

### 1️⃣ Data Preparation (Power Query & DAX)
*   Connected to the **AdventureWorks SQL Server database** within Power BI.
*   Selected and imported tables and columns pertinent to the **Purchasing** analysis.
*   Performed necessary data type transformations and handled missing values using **Power Query Editor**.
*   Created essential calculated columns and **DAX measures** for key procurement metrics (e.g., `Total Purchase Cost (YTD)`, `Average Lead Time Overall`).
*   Established and verified relationships between tables in the Power BI data model to ensure analytical integrity.

### 2️⃣ Power BI Visualization & Dashboarding
Developed interactive and insightful dashboards tailored to specific stakeholder needs, focusing on clear data presentation and actionable insights.

---

## 📊 Key Insights & Visualizations

🔍 **Dashboard Previews & Analysis**

The procurement operations dashboard is structured into user-centric pages:

### **Page 1: Purchasing Overview - Cost & Volume**
<p align="center">
  <img src="https://github.com/user-attachments/assets/81ac067f-0ad7-497f-84fc-950611f675fd" alt="Purchasing Overview: Cost & Volume Dashboard" width="700">
</p>

📌 **Analysis (Cost & Volume):**
*   **Observations:** Ordering activities and associated costs display distinct **seasonal patterns**, notably a dip in Q3-early Q4. **"Components"** emerge as a primary driver of purchasing expenditure.
*   **Recommendations:** Strategically optimize procurement costs for "Components." Align inventory planning with identified seasonal trends. Closely monitor months showing high "Cost Impact by Price."

### **Page 2: Purchasing Operations - Efficiency, Details & Vendor Insights**
<p align="center">
  <img src="https://github.com/user-attachments/assets/32ff243f-1e3a-41f4-a900-f190b3c50d11" alt="Purchasing Operations: Efficiency & Details Dashboard" width="700">
</p>

📌 **Analysis (Operational Efficiency & Delivery):**
*   **Observations:** An evident need exists to **shorten order-to-ship (lead) times**. The effectiveness of different shipping methods (balancing cost and speed) requires thorough analysis. A notable drop in average order value was observed in October.
*   **Recommendations:** Prioritize initiatives to **optimize lead times**. Evaluate and select shipping methods offering the best cost-speed equilibrium. Review order consolidation strategies. Consistently monitor freight and tax costs.

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
