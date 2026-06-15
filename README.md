# 🎓 Marketing ROI Optimization for Higher Education

## Overview

This Power BI project analyzes the effectiveness of marketing investments across academic programs and evaluates their impact on student admissions.

The solution combines admissions, lead generation, and marketing spend data to help decision-makers identify high-performing programs, optimize budget allocation, and improve enrollment outcomes.

The dashboard provides insights into:

* Admission trends
* Marketing efficiency
* Lead-to-admission conversion performance
* Program-level growth opportunities
* Cost optimization opportunities
* Strategic enrollment planning

---

# Business Objective

Higher education institutions invest significant marketing budgets across multiple programs. However, determining which programs generate the highest returns can be challenging.

This project was developed to answer key business questions:

* Which programs generate the highest admissions?
* Which programs deliver the best return on marketing investment?
* How efficiently are leads converted into admissions?
* Which programs require budget optimization?
* Where should future marketing investments be focused?

---

# Dataset Overview

The dataset contains information related to:

* Academic Programs
* Program Groups
* Marketing Drives
* Academic Years
* Lead Volumes
* Admissions
* Marketing Spend

The model enables comparative analysis between 2024 and 2025 performance.

---

# Data Model

The solution follows a Star Schema architecture to improve performance and maintain scalability.

### Fact Table

* Fact_ProgramAnalysis

### Dimension Tables

* Dim_Program
* Dim_Group
* Dim_Drive
* Dim_AcademicYear

### Model Highlights

* Star Schema Design
* One-to-Many Relationships
* Optimized Query Performance
* Scalable Reporting Structure
* Dynamic Filtering Support

![Data Model](Documentation/Data_Model.png)

---

# Dashboard Pages

## 1. Executive Dashboard

Provides a consolidated view of overall marketing and admissions performance.

### Key Metrics

* Total Admissions
* Total Leads
* Total Marketing Spend
* Cost Per Admission (CAC)
* Cost Per Lead (CPL)
* Conversion Rate

### Business Value

Enables leadership teams to quickly assess enrollment performance and marketing effectiveness.

![Executive Dashboard](Dashboard_Screenshots/Executive_Dashboard.png)

---

## 2. Year-over-Year Performance Analysis

Compares 2024 and 2025 performance across programs and groups.

### Analysis Included

* Admissions Growth
* Lead Growth
* Spend Growth
* Group-Level Performance Comparison

### Business Value

Identifies growth trends and highlights areas requiring intervention.

![Year-over-Year Analysis](Dashboard_Screenshots/YoY_Trends.png)

---

## 3. Program Performance Analysis

Provides detailed program-level performance insights.

### Analysis Included

* Admissions Growth %
* Lead Growth %
* Conversion Rate Changes
* Cost Per Lead Changes
* Cost Per Admission Changes

### Business Value

Helps identify top-performing and underperforming academic programs.

![Program Analysis](Dashboard_Screenshots/Program_Analysis.png)

---

## 4. Marketing Efficiency Analysis

Evaluates the relationship between marketing investment and admissions outcomes.

### Analysis Included

* Cost Per Admission vs Admissions Matrix
* High Potential Programs
* Growth Opportunity Identification
* Budget Optimization Opportunities

### Business Value

Supports data-driven marketing budget allocation.

![Marketing Efficiency Analysis](Dashboard_Screenshots/Marketing_Efficiency.png)

---

## 5. Lead-to-Admission Conversion Analysis

Examines the effectiveness of the enrollment funnel.

### Analysis Included

* Lead-to-Admission Funnel
* Conversion Rate by Program
* Lead Volume vs Conversion Efficiency
* Funnel Bottleneck Identification

### Business Value

Highlights opportunities to improve enrollment conversion performance.

![Lead Conversion Analysis](Dashboard_Screenshots/Lead_Conversion_Funnel.png)

---

# Key KPIs

### Enrollment Metrics

* Total Admissions
* Admissions Growth %
* Program-wise Admissions

### Marketing Metrics

* Marketing Spend
* Cost Per Lead (CPL)
* Cost Per Admission (CAC)

### Conversion Metrics

* Lead Volume
* Conversion Rate %
* Conversion Growth %

---

# Key Insights

### Admissions Performance

* Significant growth observed across multiple programs in 2025.
* M.Tech AI-related programs emerged as major contributors to admissions growth.
* Program performance varies significantly across academic groups.

### Marketing Efficiency

* Higher spend does not always translate into higher admissions.
* Several programs demonstrate strong performance with comparatively lower acquisition costs.
* Budget optimization opportunities exist across multiple portfolios.

### Conversion Performance

* Overall lead-to-admission conversion rate stands at approximately 4.31%.
* Certain programs achieve substantially higher conversion rates than the portfolio average.
* Improving conversion efficiency presents a major opportunity for enrollment growth.

---

# Skills Demonstrated

### Power BI

* Interactive Dashboard Development
* KPI Design
* Data Visualization
* Performance Optimization

### Data Modeling

* Star Schema Design
* Relationship Management
* Dimensional Modeling

### DAX

* Time Intelligence
* Growth Calculations
* Conversion Metrics
* Variance Analysis

### Business Analytics

* Marketing Analytics
* Enrollment Analytics
* Funnel Analysis
* Strategic Decision Support

---

# Tools & Technologies

* Power BI Desktop
* DAX
* Power Query
* Data Modeling
* Business Intelligence
* Data Visualization

---

# Repository Structure

```text
Marketing-ROI-Optimization-for-Higher-Education
│
├── README.md
│
├── Documentation
│   └── Data_Model.png
│
└── Dashboard_Screenshots
    ├── Executive_Dashboard.png
    ├── YoY_Trends.png
    ├── Program_Analysis.png
    ├── Marketing_Efficiency.png
    └── Lead_Conversion_Funnel.png
```

---

# Author

### Gourav Dutta

Data Analyst | Power BI Developer | Business Intelligence Enthusiast

GitHub: https://github.com/gouravinsights


