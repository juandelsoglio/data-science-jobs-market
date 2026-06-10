# Data Science Jobs Market — End-to-End Power BI Project

## Project Description
This repository contains a full Business Intelligence project analyzing a dataset of 3,755 data science professionals worldwide. The project goes from raw data processing and structural database normalization to custom data modeling (Star Schema), advanced analytics using DAX, and a professional 5-page interactive dashboard.

---

## Data Architecture & Normalization
The original flat dataset was denormalized and structured into a relational model consisting of **9 interconnected tables** to optimize performance, avoiding redundant data and ensuring information tracing:
* **Fact Table:** `EMPLEADOS` (12 attributes including composite FKs, metrics, and hiring timestamps).
* **Dimension Tables:** `EMPRESAS`, `GÉNERO`, `EXPERIENCIA`, `TIPO EMPLEO`, `MONEDA SALARIO`, `PAÍS RESIDENCIA`, `LOCALIZACIÓN`, and `TAMAÑO COMPAÑÍA`.
* **Time Intelligence:** Integrated a custom corporate `_Calendario` table to track time-based trends natively.

### Relational Model (Star Schema) in Power BI:
![Data Model Schema](data_model_star_schema.png)

---

## Advanced Analytics & DAX Implementation
Over 15 custom DAX measures and advanced conditional columns were developed for strategic reporting, using functions like `CALCULATE`, `SWITCH`, `AVERAGE`, and `COUNT`. 

### Key DAX Engineering Features:
* **Dynamic Segments:** Created custom job filters (`_¿Es TOP 5?`) to isolate core industry roles representing 76.8% of market volume.
* **Workplace Categorization:** Normalized remote percentage indicators into descriptive operational profiles (`Presencial`, `Híbrido`, `Remoto`).

### Technical Code & Formulas Preview:
![DAX Formulas](dax_formulas_preview.png)

---

## Interactive Dashboard UI/UX

The dashboard was built following modern interface rules, implementing intuitive button navigation, unified branding colors (`#2C87BF`, `#262626`), and metric monitors for decision-makers.

### 1. Global Fleet Analytics (Executive Summary)
Tracks primary market markers like total records, overall salary averages ($137,570 USD), and seniority gauges.
![Dashboard Overview](dashboard_overview.png)

### 2. Deep-Dive Role Trends & Workplace Modalities
Analyzes year-over-year hiring acceleration from 2020 to 2023, confirming sector growth and tracking remote vs. on-site ratios.
![Role Analytics](top_roles_analysis.png)

---

## Repository Contents
* `Data_Science_Jobs_Market.pbix`: The source Power BI file with queries, relationships, and visual pages.
* `dashboard_overview.png`: Executive dashboard interface view.
* `top_roles_analysis.png`: Role and modality trend analytical view.
* `data_model_star_schema.png`: Relational star schema diagram layout.
* `dax_formulas_preview.png`: Snippet of technical calculations.

## Source Dataset
Data obtained from Kaggle (Global Data Science Salaries Public Records).
