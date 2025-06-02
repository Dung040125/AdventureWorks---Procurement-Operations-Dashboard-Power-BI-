# 📊 AdventureWorks Industry Procurement Analysis - Power BI
<p align="center">
  <img src="https://github.com/user-attachments/assets/23b1ad67-fc1d-4124-8efe-d04eb1acdcf6" alt="AdventureWorks Project Banner" width="1000"> 
</p>

* **Author:** Nguyen Thi Thuy Dung
* **Date:** 2025-04
* **Tools Used:** Microsoft Power BI, DAX, Excel (for Design Thinking), SQL (SQL Server)

---

## 📑 Table of Contents
[📌 Background & Overview](#-background--overview)  
[📂 Project Focus & Dataset Context](#-project-focus--dataset-context)  
[🧠 Design Thinking Process](#-design-thinking-process)  
[⚒️ Main Process: Data Preparation & Dashboard Development](#%EF%B8%8F-main-process-data-preparation--dashboard-development)  
[📊 Key Insights & Visualizations](#-key-insights--visualizations)  
[🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)  
[🚀 Usage Instructions](#-usage-instructions)  
[📂 Project Deliverables](#-project-deliverables)  
[💡 Design Discussions and Decisions](#design-discussions-and-decisions)

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
## 💾 Data Model
The data model for this project establishes relationships between the dimension and fact tables listed above. This structure is crucial for enabling efficient querying and accurate analysis in Power BI.
The diagram below illustrates the relationships between these tables within the Power BI environment:

<p align="center">
  <img src="https://github.com/user-attachments/assets/4eeaf36b-5634-49e4-bbcb-7f2ffb90cdc5" alt="AdventureWorks Procurement Data Model Relationships" width="1000">
</p>

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
The company's procurement operations are **large-scale** (total historical cost **$70.48M**, average PO value **$17.57K**) and follow **clear seasonal cycles**, with costs **peaking in June** ($8.08M) and decreasing towards the end of Q3. Notably, **24.6% of total purchase costs are concentrated within the Top 5 vendors** ($17.36M), highlighting the importance of managing relationships with these strategic partners.

*   #### **Optimize Costs & Manage Strategic Vendor Relationships:**
    *   The fact that **a quarter of spending is focused on the Top 5 vendors** (including **"Chicago City Saddles"**) underscores the opportunity for **better price negotiations** and **building stronger partnerships** to ensure stable supply and competitive pricing.
    *   The strategic product **"ProductID 528"** (50 distinct orders, 150 total units), which is closely monitored and potentially linked to these top vendors, also follows the general seasonal trend.
    *   💡 
        *   Regularly evaluate the performance of the Top 5 vendors. Leverage significant purchasing power to **negotiate more favorable terms**.
        *   Further analyze the link between "ProductID 528" and top vendors to **optimize ordering processes and costs** for this critical product, especially during peak seasons.

*   #### **Leverage Seasonal Trends & Price Optimization Capabilities:**
    *   Monthly cost fluctuations are primarily driven by **changes in order volume**. However, there are positive indications that **"price" (encompassing base price, taxes, and fees) tends to decrease or have a cost-reducing impact in later months**, suggesting cost optimization capabilities.
    *   💡
        *   Plan budgets and procurement forecasts based on **clear seasonal trends** (peak in June, low towards end-Q3) for effective cash flow management.
        *   Investigate and **replicate factors contributing to "price" reduction in later months** for other periods, possibly through early ordering or strategic timing of purchases.

### **Page 2: Purchasing Operations - Efficiency, Details & Vendor Insights**
<p align="center">
  <img src="https://github.com/user-attachments/assets/5a9319a0-00b4-42c9-b0aa-0e1dbfb611d9" alt="Purchasing Operations: Efficiency & Details Dashboard" width="900">
</p>

📌 **Analysis (Operational Efficiency & Delivery):**
The company's operational efficiency and delivery demonstrate **stability and good control** across various aspects: from core product unit prices (average **38.16**), average overall lead time (**19.45 days**), to ancillary cost rates (freight ~2.48%, tax ~8.00%) remaining stable across months. The business also prioritizes specific shipping methods (IDs 5 & 4 account for the majority of orders), indicating optimization in transport channels.

*   #### **Maintain Stability & Optimize Existing Processes:**
    *   The stability of core product prices and ancillary costs allows for **more accurate procurement cost forecasting**. Internal order processing time is quite stable (averaging **~9 days**).
    *   Having **86 active vendors in the most recent year (2014)** indicates a diversified supply base, which helps mitigate risks.
    *   💡
        *   Continue maintaining good relationships with suppliers to ensure stability in pricing and lead times.
        *   Closely monitor the **slight increase in order processing time to 9.22 days in November**; investigate the cause (possibly due to year-end workload) and implement corrective measures to maintain operational efficiency.

*   #### **Leverage Opportunities from High-Value Transactions & Seasonal Optimization:**
    *   While order volumes might decrease in certain months, **October stands out with a significantly high average order value (over $20K)**, suggesting strategic purchases or procurement of high-value items concentrated during this period.
    *   💡
        *   Further analyze high-value orders in October: this presents an opportunity to **negotiate better terms** or **plan cash flow effectively** for these large transactions.
        *   In conjunction with seasonality insights from cost analysis, assess whether concentrating high-value orders in October is the optimal strategy or if they could be more evenly distributed.
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
