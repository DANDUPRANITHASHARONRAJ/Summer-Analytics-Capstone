# Summer-Analytics-Capstone
# 🚗 Dynamic Pricing for Urban Parking Lots

**Capstone Project — Summer Analytics 2025**  
Hosted by Consulting & Analytics Club × Pathway  
**Team:** [DANDU PRANITHA SHARON]  
**Email:** [s.dandu@iitg.ac.in]

---

## 🧾 Project Overview

Urban parking often faces inefficiencies due to fixed pricing, leading to overcrowding or underutilization. This project aims to solve that by building a **real-time dynamic pricing system** for 14 urban parking lots using data-driven demand estimation and economic logic.

Using features such as:
- Occupancy levels
- Queue lengths
- Traffic congestion
- Vehicle types
- Special events/holidays

we estimate **parking demand** and adjust prices dynamically every 30 minutes using a weighted demand function and base price of $10.

---

## 🛠️ Tech Stack

| Tool / Library | Purpose |
|----------------|---------|
| **Python**     | Core programming language |
| **NumPy, Pandas** | Data processing, math |
| **Pathway**    | Real-time streaming, stateful pipeline |
| **Bokeh**      | Interactive data visualization |
| **Google Colab** | Cloud-based notebook development |
| **GitHub**     | Version control and submission |

---

## 🏗️ Architecture Diagram

A visual overview of the system's architecture is available here:  
👉 [**View Architecture Diagram**](https://www.mermaidchart.com/app/projects/5d1ed5ac-1f08-4e69-8cc4-a79019c18f36/diagrams/017e644a-80e5-4510-8e63-a5131685c509/version/v0.1/edit)

```mermaid
graph TD
    A[dataset.csv - Raw Input] --> B[Pathway Stream Processor]
    B --> C[Schema Definition]
    C --> D[Feature Engineering]
    D --> E[Demand Score Calculation]
    E --> F[Dynamic Pricing Logic]
    F --> G[Real-Time Price Output]
    G --> H[Bokeh Visualization - Optional]
