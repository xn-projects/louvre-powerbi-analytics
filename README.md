# Louvre Power BI Analytics Dashboard (2018–2024)

This repository contains a **Power BI analytics case study** focused on visitor behavior, revenue performance, exhibitions, and digital audience growth of the **Louvre Museum**.

The project was designed as a **management-level BI solution**, not a training dashboard, with an emphasis on data modeling, analytical logic, and usability.

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

High-level KPIs and long-term trends:

- Total Visits  
- Exhibition Attendance  
- Visitor Satisfaction (%)  
- Total Revenue  
- Ticket Sales Revenue  
- Auditorium Visits  
- School Visits  
- Free Admission Share (%)  

[`images/overview.png`](images/overview.png)

---

### 2️⃣ Social Media

Digital audience and website traffic analysis:

- Platform growth comparison  
- Year-over-year trends  
- Website traffic dynamics  

[`images/social_media.png`](images/social_media.png)

---

### 3️⃣ Exhibitions

Exhibition performance analytics:

- Exhibition attendance (selected year)  
- Total number of exhibitions  
- Artworks and artworks from the Louvre collection  
- Top exhibitions by attendance and historical performance
  
[`images/exhibitions.png`](images/exhibitions.png)

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
