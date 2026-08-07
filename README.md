# 🛒 Amazon Workforce & Sales Intelligence Dashboard
*A dynamic Excel dashboard transforming raw Amazon sales data into actionable retail insights.*

---

## 1. Short Description / Purpose
This project acts as a comprehensive sales and workforce intelligence tool designed for a retail tech company. Built from a raw dataset of 100 sales transactions across multiple regions, products, and customer profiles, this project demonstrates end-to-end data processing. The core objective is to allow management to explore customer trends, evaluate fulfillment efficiency, and track revenue generation through an interactive, automated dashboard.

---

## 2. Tech Stack & Excel Tools Used
* **Data Processing & Cleaning:** Text formatting, date parsing, handling blanks, and standardizing entries.
* **Formulas & Functions:** `XLOOKUP`, `IF`, `IFERROR`, `SUM`, `COUNT`, `AVERAGE`.
* **Data Modeling:** Combining relational tables (Sales, Customers, Products, and Region Goals) into a single cohesive Master Table.
* **Analysis:** Pivot Tables, Calculated Fields (e.g., *Effective Sales*), Grouping (e.g., Dates into Months).
* **Visualization:** Interactive Pivot Charts, KPIs, and Slicer-based filtering.

---

## 3. Data Source
* **Source Dataset:** Amazon Sales dump combined with Master Sheets for Customers, Products, and Regional Goals.
* **Structure:** Multi-sheet relational data covering Orders, Deliveries, Fulfillment Partners, Payment Methods, and Customer Demographics.

---

## 4. Key Metrics & Logic
To create accurate KPIs, custom logic and cross-referencing were applied to the raw data:
* **Delivery Performance:** Built a custom classification using `=IF([Delivery Date]-[Order Date] <=2, "Fast", "Slow")` to track supply chain efficiency.
* **Effective Sales:** A calculated field determining the revenue strictly from *Delivered* orders (excluding cancellations).
* **Cancellation Rate:** Tracked cancelled orders against total orders by region.
* **Customer Integration:** Used `XLOOKUP` to seamlessly map Customer Names from the `CustomerMaster` sheet into the raw sales data based on `Customer ID`.

---

## 5. Business Impact & Brainstorming Insights
The analysis of the dataset revealed several key business insights:
* **Top Performing Category:** The most successful product category is **Electronics**, generating a total Order Value of **$15,209** (of which $6,126 resulted in Effective Sales).
* **Risk Identification (Cancellations):** The **North Region** experiences the highest order cancellation rate at **10%** (10 out of 100 orders), resulting in $3,461 of lost/reversed revenue.
* **Strategic Value:** The dashboard allows travel operators, regional managers, and marketing teams to filter immediately by Payment Method and Delivery Status to pinpoint supply chain bottlenecks and profitable regions.

---

## 6. Dashboard Preview
<img width="1914" height="847" alt="Screenshot 2026-08-07 220043" src="https://github.com/user-attachments/assets/f8664fe3-437b-4f05-be72-d4c67e0517d1" />

