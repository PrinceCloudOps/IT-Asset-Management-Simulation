# IT Asset Management & Procurement Simulation

## 📌 Project Overview
This project is a comprehensive simulation of an **IT Asset Management (ITAM)** and **Procurement** workflow, designed for a high-volume Help Desk environment (modeled after a technical support role at Trinity Church NYC). It demonstrates the ability to manage the full hardware lifecycle, coordinate with vendors via Purchase Orders (POs), and automate KPI reporting using Microsoft Excel.

---

## 🛠️ Core Functional Components

### 1. Master Inventory Management
A centralized database used to track the organization’s hardware assets from deployment to retirement.
* **Asset Identification:** Implementation of a unique Asset ID system (e.g., TRIN-101) to ensure data integrity.
* **Lifecycle Tracking:** Real-time monitoring of device status (Deployed, In Storage, Repair, Retired).
* **Departmental Mapping:** Categorization of assets by department (Clergy, Finance, Facilities) for faster support response.

> **View Master Inventory <img width="638" height="119" alt="Inventory" src="https://github.com/user-attachments/assets/cdff7ad1-eebc-43bf-a477-b36c81c5b5a8" />:**
> 

---

### 2. Procurement & Vendor Workflow
A dedicated tracking system for IT acquisitions and vendor relationships.
* **Purchase Order (PO) Management:** Documentation of orders including PO numbers, quantities, and item descriptions.
* **Vendor Coordination:** Management of orders from major vendors such as Dell, Apple, and CDW.
* **Budget Tracking:** Automated calculation of total costs per order to maintain fiscal oversight.

> **View Procurement Log <img width="567" height="99" alt="Procuremnet" src="https://github.com/user-attachments/assets/ba4dc363-2668-4837-8104-220a65456f3e" />:**
> 

---

### 3. Automated KPI Dashboard
An executive-level reporting tool that provides real-time visibility into departmental health and SLA compliance.
* **Live Metrics:** Utilizes `COUNTA`, `SUM`, and `COUNTIF` formulas to bridge data from the Inventory and Procurement sheets.
* **SLA Monitoring:** Tracks "Critical Repairs" and "Resolution Rates" to ensure organizational targets are met.
* **Spend Analysis:** Aggregates total procurement spending against a defined $10,000 budget.

> **View Metrics Dashboard:**
> <img width="448" height="100" alt="Dashboard" src="https://github.com/user-attachments/assets/457ae547-da49-413b-ba84-84df3369428a" />

---

## 🧠 Technical Skills & Formulas Demonstrated
This project showcases "Strong Excel Skills" as required in modern Technical Support roles:

* **Asset Counting:** `=COUNTA(Inventory!A:A)-1` (Automated inventory tracking).
* **Conditional Reporting:** `=COUNTIF(Inventory!F:F, "Repair")` (Identifying critical hardware failures).
* **Financial Summation:** `=SUM(Procurement!F:F)` (Real-time budget tracking).
* **Data Visualization:** Implementation of filters and conditional formatting to highlight items requiring immediate action.

---

## 🚀 How to Use This Simulation
1. **Procurement:** Log a new order in the `Procuremnet` sheet. Once the status changes to "Received," the hardware is ready for deployment.
2. **Inventory:** Assign the new device an Asset ID in the `Inventory` sheet and update the user/department fields.
3. **Reporting:** Monitor the `Dashboard` to see the "Total Inventory Count" and "Total Spend" update automatically based on your entries.
