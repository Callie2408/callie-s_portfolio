# callie-s_portfolio
Analytics Portfolio


# Power BI

This repository contains a Power BI project focused on
business-oriented data analysis and reporting.

---

## SLA Performance & Ticket Management Dashboard

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

- Star schema structure linking ticket fact table to dimension tables. Designed to enable efficient filtering and time-based analysis. Data was merged and cleansed in Power Query.

<p align="center">
  <img src="Data-Modelling.png" width="900">



  
**Key Insights**
- Majority of tickets meet SLA for resolution, but assessment within 2 days shows occasional drops (~94% in some months). A KPI alert was created in Power BI Service to notify managers of SLA breaches
- Ticket volume is relatively stable with seasonal fluctuations around August and December.
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

<br>
<br>
<br>

---

<br>
<br>
<br>

## Time Booking Performance & Resource Optimisation Dashboard

**Objective**

Deliver a scalable self-service solution through Power BI that replaces manual Excel reporting, driving real-time visibility of time booking and enabling better resourcing decisions, improved utilisation, and stronger financial control.

**Key questions**
- Are employees overbooking or underbooking against contracted hours?
- Which contracts are over- or under-resourced?
- How much time is booked to recoverable vs non-recoverable (overhead) codes?
- Who has missing or late timesheet submissions?
- How does actual booking compare to forecasted/assigned hours?
- Which teams or individuals are driving discrepancies?



**Data Cleanse**

Standardised and cleaned the data across multiple datasets in Power Query. This included removing duplicate entries, normalising columns to ensure accurate joins, transforming date field to support time-based analysis, validating mappings and reducing unnecessary columns/ cardinality


**Core Visuals**

<p align="center">
  <img src="Timesheet Dashboard.png" width="900">
</p>

**Data Model**

- Developed a star schema for improved performance and scalability. Integrated additional datasets (contract pipeline / assigned hours) to enable forecast comparisons. Established relationships using unique keys and validated join integrity

<p align="center">
  <img src="Data Model - Resourcing Dashboard.png" width="900">


**DAX Calculations**
- Calculated the % of codes booked that are recoverable.
  
<p align="center">
  <img src="DAX - Resourcing Dashboard.png" width="900">

<br>
<br>
<br>

- Calculates the volume of contracts booked.
  
<p align="center">
  <img src="DAX 2 - Resourcing Dashboard.png" width="900">

  
**Key Insights**
- A significant proportion of hours were consistently booked to overhead rather than recoverable work
- Multiple contracts showed persistent underbooking, indicating potential resourcing gaps
- A small number of employees contributed disproportionately to overbooking instances
- Certain JA codes (e.g. support/non-productive) dominated time allocation
- Forecast vs actual analysis highlighted misalignment between planned and delivered effort
- Booking compliance varied significantly between teams, highlighting inconsistent behaviours
- Certain JA codes were misaligned to overhead or recoverable



**Recommendations**
- Strengthen governance through standardised JA codes, improved booking practices, and clear categorisation of overhead, recoverable, and customer work
- Introduce monitoring to drive accountability and visibility of booking behaviour
- Use alerts to proactively flag missing, late, or non-compliant timesheet entries
- Investigate underbooked contracts to determine whether there are resourcing gaps or reduced demand are the root cause
- Analyse high overhead usage at employee level to identify opportunities to improve utilisation and financial performance



**Skills & Tools demonstrated**
- Power BI (data modelling, DAX, visual design, performance optimisation)
- Power Query (data transformation, cleansing, merging datasets)
- Data Modelling (star schema, relationships, optimisation techniques)
- Stakeholder Management (requirements gathering, iterative delivery, feedback loops)
- Business Understanding (resource management, utilisation, financial governance)


<br>
<br>
<br>

---

<br>
