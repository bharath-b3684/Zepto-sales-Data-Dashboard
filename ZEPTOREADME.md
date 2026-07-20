# Zepto Sales Data Dashboard: Quick-Commerce Operations Analytics

An end-to-end data analytics project focused on auditing, cleaning, and visualizing quick-commerce fulfillment cycles. This project transforms raw delivery logs into a dynamic, interactive performance dashboard using Microsoft Excel to uncover core revenue trends and operational friction points.

---

## 📌 Project Overview
In the hyper-growth quick-commerce sector, tracking order metrics, regional performance, and rider cycles determines profitability. This project evaluates a dataset containing **1,500 delivery profiles** across major Indian hubs[cite: 5]. By leveraging automated data cleansing pipelines and relational PivotTable schemas, it consolidates thousands of rows into a streamlined, high-level business intelligence cockpit.

### Core Objectives
* **Data Sanitization:** Resolve text schema anomalies, eliminate phantom space boundaries, and rectify missing geolocation fields to ensure reporting accuracy.
* **Interactive Architecture:** Deploy a centralized, multi-chart dashboard managed via interconnected structural slicer menus for fast, no-code data exploration.
* **Operational Diagnostics:** Isolate systemic patterns in order cancellations, transit time delays, and localized demand trends to suggest actionable supply chain solutions.

---

## 🛠 Tools & Tech Stack
* **Microsoft Excel:** Data profiling, string manipulation, and PivotTable aggregates.
* **Excel Slicers:** Connected dashboard control layers via report connection synchronization.
* **Markdown/Word:** Structured technical report compilation.

---

## 🧹 Data Cleaning Pipeline
Raw transaction logs frequently present formatting issues that disrupt downstream analytics. The following preprocessing fixes were executed before chart compilation:
* **String Standardization:** Applied text trimming to erase leading and trailing whitespace variances inside product categories and payment entries (e.g., merging split entries for consistency).
* **Missing Field Remediation:** Identified and isolated 28 records missing localized city identifiers, mapping them accurately to eliminate 'N/A' layout options inside filtering tools[cite: 5].
* **Boundary Cleanup:** Pruned blank phantom rows sitting at the bottom of the data range to prevent zero-value distortion in pivot summaries.
* **Logic Auditing:** Cross-referenced rows missing transit durations to confirm an exact, absolute alignment with canceled/failed delivery states.

---

## 📊 Summary Data Profiles

### 1. Regional Sales Distribution
| City Location | Total Revenue Generated (INR) |
| :--- | :--- |
| **Bangalore** | 201,866.19 |
| **Delhi** | 180,570.60 |
| **Mumbai** | 169,384.46 |

### 2. Order Fulfillment Integrity
| Fulfillment Status | Number of Orders |
| :--- | :--- |
| **Delivered Successfully** | 1,256 |
| **Cancelled** | 114 |
| **Failed** | 82 |
| **Returned** | 48 |

---

## 💡 Key Business Insights
* **Primary Volume Anchors:** Bangalore acts as the highest producing market, contributing over 201,000 INR in revenue, with Delhi and Mumbai tracking closely behind[cite: 5].
* **Systemic Revenue Leakage:** Approximately 13% of all simulated orders fall out of the standard fulfillment cycle, primarily driven by 114 cancellations and 82 technical or operational order failures[cite: 5].
* **Fulfillment Latency:** Across all successful deliveries, the average delivery velocity maintains a steady baseline of 24.66 minutes, though heavy rush-hour slots present significant speed degradation[cite: 5].
* **High-Velocity Categories:** Fast-moving consumer goods—specifically fresh produce, snacks, and daily beverage items—consistently outperform baked goods and specialty segments in volume frequency.

---

## 📈 Strategic Recommendations

### 🛡️ Mitigate Order Cancellations
Address the 114 canceled orders by instituting stronger transit packaging standards at the dark-store phase[cite: 5]. Internal remarks trace a large percentage of cancellations to physical item damage during high-speed transit.

### 📍 Rectify Logistics Failures
The 82 failed deliveries represent an immediate loss of rider time and direct fuel spend[cite: 5]. Implementing mandatory geolocation validation at the customer checkout phase will structurally lower address routing drops.

### ⚡ Regional Stock Optimization
Allocate priority warehouse supply depth to Bangalore dark stores. Since Bangalore represents the highest grossing region, maintaining zero-stockout conditions for fast-moving items will protect high-margin loops[cite: 5].

### 🔒 Enforce Data Validation at Entry
Implement structured input validation on the consumer app to ensure fields like "City" are mandatory, permanently blocking the formatting defects that caused the missing row data fixed during this cycle[cite: 5].

---

## 🖥️ Dashboard Architecture & Usage
The final Excel dashboard is built with user experience in mind, allowing stakeholders to filter data instantly without deep technical knowledge:
1. **Dynamic Top Navigation:** Three horizontally arranged slicers allow instant cross-filtering by **Order Month**, **City**, and **Category**.
2. **Synchronized Cross-Filtering:** All chart objects update dynamically in unison when a button is clicked.
3. **Clean Visual Hierarchy:** Default harsh borders and system-heavy color presets were removed, opting for a professional navy corporate presentation.

### How to Explore the Dashboard:
1. Download the `Zepto_Sales_Data_Dashboard.xlsx` file from the file list above.
2. Open the file in Microsoft Excel.
3. Use the soft-colored buttons at the top of the workspace to filter by city or product category and watch the data update instantly.
