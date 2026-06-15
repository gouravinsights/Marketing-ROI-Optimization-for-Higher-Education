# 🎓 Marketing ROI Optimization for Higher Education

## 📌 Project Overview

This Power BI solution analyzes marketing effectiveness across academic programs and evaluates how marketing investments influence student admissions.

The dashboard helps decision-makers:

* Identify high-performing programs
* Measure marketing ROI
* Analyze lead-to-admission conversion efficiency
* Optimize budget allocation
* Improve enrollment outcomes

---

## 🚀 Business Problem

Educational institutions invest significant budgets in marketing campaigns, but determining which programs generate the best admissions outcomes remains challenging.

This project provides a data-driven framework to evaluate:

* Marketing Spend
* Leads Generated
* Admissions Achieved
* Cost Per Lead (CPL)
* Cost Per Acquisition (CPA)
* Conversion Efficiency
* Program Performance Trends

---

## 🛠 Tools & Technologies

* Power BI
* DAX
* Power Query
* Data Modeling
* Star Schema Design
* Business Intelligence

---

## 📊 Data Model

The solution follows a Star Schema design with a centralized fact table and supporting dimension tables.

### Fact Table

* Fact_ProgramAnalysis

### Dimension Tables

* Dim_Program
* Dim_Group
* Dim_Drive
* Dim_AcademicYear

![Data Model](Documentation/Data_Model.png)

---

## 🏗 Solution Architecture

The solution follows a structured Business Intelligence workflow from raw data ingestion to executive-level reporting.

![Architecture](Documentation/Project_Architecture.png)

---

## 📈 Key KPIs

### Marketing Metrics

* Total Spend
* Cost Per Lead (CPL)
* Cost Per Acquisition (CPA)

### Admissions Metrics

* Total Admissions
* Admissions Growth %
* Conversion Rate %

### Lead Metrics

* Total Leads
* Lead Growth %
* Lead-to-Admission Conversion %

---

# Sample DAX Measures

The dashboard leverages DAX measures to calculate business KPIs, evaluate marketing efficiency, and identify program performance trends.

### Total Admissions

```DAX
Total Admissions =
SUM(Fact_ProgramAnalysis[B2C Admissions])
```

### Conversion Rate

```DAX
Conversion % =
DIVIDE(
    [Total Admissions],
    [Total Leads],
    0
)
```

### Cost Per Lead (CPL)

```DAX
Cost Per Lead =
DIVIDE(
    [Total Spend],
    [Total Leads],
    0
)
```

### Cost Per Acquisition (CPA)

```DAX
Cost Per Acquisition =
DIVIDE(
    SUM(Fact_ProgramAnalysis[Spends]),
    SUM(Fact_ProgramAnalysis[B2C Admissions]),
    0
)
```

### Admissions Growth %

```DAX
Admissions Growth % =
DIVIDE(
    [2025 Admissions] - [2024 Admissions],
    [2024 Admissions],
    0
)
```

### Performance Classification

```DAX
Performance Gap =
SWITCH(
    TRUE(),
    [Admissions Change %] >= 0.50, "Exceeding Market Expectations",
    [Admissions Change %] >= 0.10, "Strong Performance",
    [Admissions Change %] > -0.10, "Stable Performance",
    [Admissions Change %] > -0.40, "Moderate Underperformance",
    "Significant Underperformance"
)
```

---

# Dashboard Pages

## 1️⃣ Executive Dashboard

Provides a high-level overview of admissions performance, marketing spend, leads, and conversion metrics.

![Executive Dashboard](Dashboard_Screenshots/Executive_Dashboard.png)

---

## 2️⃣ Year-over-Year Trend Analysis

Compares 2024 and 2025 performance across admissions, leads, and marketing spend.

![YoY Trends](Dashboard_Screenshots/YoY_Trends.png)

---

## 3️⃣ Program Performance Analysis

Evaluates individual program performance and identifies growth opportunities.

![Program Analysis](Dashboard_Screenshots/Program_Analysis.png)

---

## 4️⃣ Marketing Efficiency Analysis

Analyzes return on marketing investment and identifies programs requiring optimization.

![Marketing Efficiency](Dashboard_Screenshots/Marketing_Efficiency.png)

---

## 5️⃣ Lead Conversion Funnel Analysis

Measures lead-to-admission conversion effectiveness across programs.

![Lead Conversion Funnel](Dashboard_Screenshots/Lead_Conversion_Funnel.png)

---

## 📌 Key Insights

* M.Tech AI & ML generated the highest admissions volume.
* Several B.Tech programs delivered strong admissions at lower acquisition costs.
* Marketing spend alone does not guarantee admissions success.
* Conversion efficiency is a major driver of enrollment performance.
* Certain programs present strong growth opportunities with optimized spending.

---

# Business Recommendations

## Optimize Marketing Spend

Programs with high acquisition costs and lower admission outcomes should undergo campaign review and budget optimization to improve ROI.

## Scale High-Performing Programs

Programs demonstrating strong admissions growth and efficient acquisition costs should receive increased marketing investment.

## Improve Conversion Efficiency

Programs generating high lead volumes but low admission conversions should focus on lead nurturing strategies and admissions counseling improvements.

## Introduce Performance-Based Budgeting

Future marketing budgets should be allocated using program performance metrics rather than equal distribution across all programs.

## Continuous KPI Monitoring

Monitor admissions, conversion rates, CPL, and CPA regularly to support proactive decision-making.

### Expected Business Impact

* Reduced student acquisition costs
* Improved marketing ROI
* Higher lead-to-admission conversion rates
* Better budget allocation
* Increased admissions growth across programs

---

## 📂 Repository Structure

```text
Assets/
│
├── Marketing_ROI_Optimization.pbix

Dashboard_Screenshots/
│
├── Executive_Dashboard.png
├── YoY_Trends.png
├── Program_Analysis.png
├── Marketing_Efficiency.png
└── Lead_Conversion_Funnel.png

Documentation/
│
├── Data_Model.png
└── Project_Architecture.png
```

---

## 👨‍💻 Author

**Gourav Dutta**

Power BI | Data Analytics | Business Intelligence

GitHub: https://github.com/gouravinsights
