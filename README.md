# callie-s_portfolio
Analytics Portfolio


# Power BI

This repository contains a Power BI project focused on
business-oriented data analysis and reporting.

---

## Ticket Dashboard

**Objective**

Analyse Ticket data to monitor SLA performance, identify delays in resolution, and highlight trends in ticket volume to support operational decision-making.

**Key questions**
- Are SLAs being met (assessment within 2 days, resolution before due date)?
- Which team members handle the highest ticket volumes?
- Is ticket demand increasing over time?
- Where are delays occurring in the ticket lifecycle?


**Core visuals**
- Tickets volumes that are Assigned, Opened and Closed
- KPI percentages


<p align="center">
  <img src="Ticket-Dashboard.png" width="900">
</p>

**Data Model**

- Star schema structure linking ticket fact table to dimension tables. Designed to enable efficient filtering and time-based analysis

<p align="center">
  <img src="Data-Modelling.png" width="900">



  
**Key Insights**
- Majority of tickets meet SLA for resolution, but assessment within 2 days shows occasional drops (~94% in some months). A KPI Alert was produced in Power BI service to notify managers of KPI Failures.
- Ticket volume is relatively stable with slight monthly fluctuations
- A small number of team members handle a disproportionate number of tickets
- Closure rates closely track ticket creation, indicating steady backlog management
- Tickets were found to be out of SLA incorrectly, due to different SLA definitions between teams.

**Recommendations**
- Investigate teams / team members with lower SLA performance to identify root causes of delays
- Review ticket distribution across employees to ensure balanced workload
- Analyse periods with SLA dips to determine if driven by volume spikes or complexity
- Introduce early warnings or alerts for tickets at risk of breaching SLA
- Introduce a consistent KPI definition across all teams to standardise performance reporting



**Skills & Tools demonstrated**
- Power BI
- Power Query (to cleanse and merge the data)
- DAX (measures, calculated columns)
- Data modelling
- Interactive dashboards (filters, drill-throughs)



---


