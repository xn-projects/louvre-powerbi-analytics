# Methodology

This document describes the **analytical approach, calculation logic, and key assumptions** applied in the Louvre Power BI Analytics Dashboard.

The focus of this methodology is to ensure **consistency, interpretability, and decision-making relevance**, rather than purely technical implementation details.

---

## 1️⃣ Analytical Scope

The analysis covers the period **2018–2024** and focuses on:
- visitor behavior and attendance
- revenue dynamics
- audience structure
- exhibition performance
- digital audience growth

The methodology was designed to support **management-level insights**, not only descriptive reporting.

---

## 2️⃣ Data Modeling Approach

The data model follows a **fact-and-dimension structure** to ensure:
- consistent aggregation across pages
- correct filtering behavior
- scalability for future extensions

Core analytical entities include:
- visitors and attendance metrics
- exhibitions
- audience segments
- geography
- digital channels

This structure allows the same KPIs to be analyzed from multiple perspectives without duplicating logic.

---

## 3️⃣ Year-over-Year (YoY) Logic

Year-over-year comparisons are calculated dynamically based on the selected year context.

Applied principles:
- each KPI is compared to its value in the previous year
- trend indicators are used to support fast interpretation:
  - ▲ increase vs previous year
  - ▼ decrease vs previous year

This approach enables quick identification of growth, decline, and structural changes over time.

---

## 4️⃣ Multi-Year Exhibitions Handling

Some exhibitions span multiple calendar years, which introduces potential risks of double counting and ambiguous year attribution.

To ensure consistent and meaningful annual comparisons, the following rule was applied:

- each exhibition is assigned to the year in which **the majority of its duration (in days)** occurred
- total exhibition duration is calculated across calendar years
- the exhibition is attributed to the year with the highest number of exhibition days
- attendance figures are reported only for the assigned year

### Museum Closures Adjustment (2020–2021)

When calculating exhibition duration, **periods of full museum closure in 2020 and 2021 were explicitly taken into account**.

- days during which the museum was officially closed were excluded from exhibition duration calculations
- only days when the exhibition was **accessible to visitors** were counted
- this adjustment ensures that exhibition duration reflects actual visitor exposure rather than calendar time

For historical analysis, cumulative attendance is calculated separately and used exclusively for long-term exhibition rankings.

This approach ensures that each exhibition is counted **once per analysis period**, while preserving analytical consistency at both annual and long-term levels.

---

## 5️⃣ Percentage-Based Metrics Notes

Audience indicators presented in **percentage format** (such as *Youth Share* and *Free Admission Share*) are based on values **directly reported in the official Louvre publications**.

- the source reports provided these metrics only in percentage form  
- absolute visitor counts were not available for these indicators  
- no additional recalculation or estimation was performed  
- the analysis assumes the correctness of the percentage calculations as reported by the museum

These metrics are used to analyze accessibility policies, education programs, and overall audience composition, while remaining consistent with officially published figures.

---

## 6️⃣ Revenue and Attendance Analysis

Revenue-related KPIs are analyzed in parallel with attendance metrics to assess:
- the relationship between visitor volume and ticket revenue
- the impact of pricing and free admission policies
- structural changes in revenue composition over time

Combined trend visualizations support interpretation beyond absolute values.

---

## 7️⃣ Digital Channels Analysis

Digital performance is analyzed through:
- social media audience growth by platform
- website traffic trends
- year-over-year changes in digital engagement

These indicators provide context for understanding how online presence supports overall visitor interest and engagement.

---

## 8️⃣ Design and Usability Principles

The dashboard design follows several key principles:
- clear visual hierarchy
- minimal visual noise
- consistent KPI naming across pages
- readability at high metric density
- fast interpretation for decision-makers

The goal was to ensure that insights can be extracted **within seconds**, without requiring detailed explanation.

---

## 9️⃣ Limitations and Assumptions

- The analysis is based on **officially published aggregated figures** provided by the Louvre Museum.
- Granular visitor-level data was not available; all insights are derived from summary-level reporting.

During data preparation, **minor discrepancies** were identified between figures reported in annual activity reports and selected official press releases.

To ensure consistency and analytical stability:
- the **annual activity reports (Rapport d’Activités)** were treated as the primary reference source
- press releases were used only as a supplementary source when additional detail or clarification was required
- no attempt was made to reconcile or override official figures beyond this source hierarchy

These assumptions and limitations were explicitly considered during modeling to minimize the risk of misinterpretation and to preserve alignment with the museum’s official reporting.

---

For details on data origins and scope, see:   
[`data_sources.md`](data_sources.md)
