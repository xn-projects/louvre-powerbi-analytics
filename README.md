# Louvre Power BI Analytics Dashboard (2018–2024)

This repository contains a **Power BI analytics case study** focused on visitor behavior, revenue performance, exhibitions, and digital audience growth of the **Louvre Museum**.

---

## Project Overview

- Time period: **2018–2024**
- Focus: visitors, revenue, exhibitions, audience structure, digital channels

**Important:**  
No ready-made dataset was used. The data was manually extracted from official Louvre publications and transformed into an analytics-ready format.

- Details about data origins:  
 [`docs/data_sources.md`](docs/data_sources.md)

- Details about calculations and analytical logic:  
 [`docs/methodology.md`](docs/methodology.md)

---

## Repository Structure

```text
louvre-powerbi-analytics/
├── powerbi/
│   └── louvre_analytics.pbix
├── data/
│   └── louvre_analytics.db
├── images/
│   ├── overview.png
│   ├── exhibitions.png
│   └── social_media.png
├── docs/
│   ├── data_sources.md
│   └── methodology.md
└── README.md
```
---

## Dashboard Pages

### 1️⃣ Overview

The Overview page provides a high-level snapshot of museum performance, combining key KPIs with trend-based visual analysis.

#### Key KPIs
- Total Visits  
- Exhibition Attendance  
- Visitor Satisfaction (%)  
- Total Revenue  
- Ticket Sales Revenue  
- Auditorium Visits  
- School Visits  
- Free Admission Share (%)  

#### Key Visuals and Insights

- **Visitors vs Ticket Revenue Over Time**  
  A combined trend analysis showing how visitor numbers and ticket revenue evolve together across years.  
  This visualization helps assess whether revenue growth is driven by attendance, pricing effects, or a combination of both.

- **Youth Share vs Free Admission (%)**  
  A comparative trend highlighting the relationship between the share of young visitors and the proportion of free admissions.  
  This chart supports analysis of accessibility policies and their impact on audience structure.

- **Visitor Origin by Country (%)**  
  A geographic distribution of visitors by country, allowing quick identification of key source markets and changes in international audience composition.

- **School Visits vs Youth Audience Trend**  
  A trend comparison between organized school visits and the overall youth audience, helping evaluate the role of educational programs in shaping long-term visitor demographics.

Together, these visuals allow decision-makers to quickly identify structural shifts, performance drivers, and potential areas for strategic action.

![`images/overview.png`](images/overview.png)

---

### 2️⃣ Social Media

The Social Media page focuses on the museum’s digital presence and its evolution over time, providing insights into audience growth and online engagement.

#### Key Metrics
- Social media audience size by platform
- Website traffic (annual)

#### Key Visuals and Insights

- **Social Media Audience Growth by Platform**  
  A multi-year comparison of audience growth across major platforms (Facebook, Instagram, LinkedIn, Twitter/X, YouTube, Weibo. WeChat).  
  This visualization highlights differences in growth dynamics and helps identify which platforms contribute most to digital reach.

- **Website Traffic Over Time**  
  An annual trend of website visits, showing how online interest in the museum evolves over time.  
  This chart supports analysis of how digital engagement aligns with on-site attendance and major exhibitions.

Together, these visuals help assess the effectiveness of digital communication channels and their role in supporting audience development.

![`images/social_media.png`](images/social_media.png)

---

### 3️⃣ Exhibitions

The Exhibitions page provides a detailed performance analysis of temporary exhibitions, combining attendance metrics with structural characteristics.

#### Key Metrics
- Exhibition Attendance (selected year)
- Total Number of Exhibitions
- Total Artworks
- Artworks from the Louvre Collection

#### Key Visuals and Insights

- **Top Exhibitions by Attendance (Selected Year)**  
  A ranking of the most visited exhibitions within the selected year, supporting evaluation of short-term exhibition performance.

- **Top Exhibitions by Total Attendance (All Years)**  
  A historical ranking based on cumulative attendance, highlighting exhibitions with long-term impact and sustained popularity.

- **Exhibition Structure Indicators**  
  Metrics such as number of artworks and exhibition duration provide additional context for attendance figures, enabling comparisons beyond raw visitor counts.

- **Multi-Year Exhibition Logic**  
  Exhibitions spanning multiple years are handled using consistent attribution rules to ensure accurate annual and historical comparisons.

This page supports strategic decisions related to exhibition planning, resource allocation, and long-term programming.
  
![`images/exhibitions.png`](images/exhibitions.png)

---

## Analytical Purpose

This dashboard supports management-level questions such as:

- How does visitor structure change over time?  
- Which exhibitions generate the highest impact?  
- How do revenue and attendance evolve together?  
- How does digital audience growth relate to visitor behavior?

---

## Tools Used

- Power BI Desktop  
- DAX (custom measures)  
- Data modeling and transformation  
- UX-oriented dashboard design  
