## SEND \& Education Analytics Platform (Hybrid LA + MAT)

### Building an Impact-Focused SEND & Education Analytics Model (Power BI + Microsoft Fabric)

With the ongoing national conversation around SEND funding pressures and sustainability of local authority budgets, the ability to measure the real impact of provision and interventions has become increasingly important.

To explore how data platforms can support this challenge, I recently completed a project exercise focused on Special Educational Needs (SEND) and education performance analytics.


This project aligns with publicly available Department for Education national statistics on Special Educational Needs; including SEN Support, EHC Plan classifications, 

and primary type of need categories reported through the school census, and builds on this as a template to build on more detailed granularity which simulates a public-sector education 

analytics environment (Local Authority + Multi-Academy Trust) with a full Medallion architecture in Microsoft Fabric and a Power BI executive reporting suite.



### What this demonstrates

- **Bronze → Silver → Gold** data engineering in Fabric (typed, standardised, conformed)

- **Star schema modelling** for education + SEND analytics

- KPI engineering for:

&nbsp; - Attendance %, Persistent Absence %

&nbsp; - Attainment At/Above %, Expected Progress

&nbsp; - Behaviour incidents and exclusions (risk indicators)

&nbsp; - SEND prevalence (SEN / EHCP), needs distribution, placement mix

&nbsp; - Funding per SEND pupil and intervention impact


### From a technical and architectural perspective, the project demonstrates:
- Star schema dimensional modelling
- DAX-driven gap and variance analysis
- Impact and efficiency scoring metrics
- Governance-aware modelling (no live pupil data used)


### Report pages (Power BI)

1\. **Cover / Navigation Hub** – KPI strip + section navigation

2\. **Executive Overview** – attendance, attainment, gaps, top schools

3\. **SEND Strategy** – needs, placements, funding, provision vs outcomes

4\. **Behaviour \& Exclusions** – severity, exclusions, safeguarding-style risk matrix

5\. **Schools \& Trusts** – benchmarking across schools and trusts, geo insights

6\. **Pupil Drill-through** – pupil journey timeline across attendance, attainment, behaviour and interventions



### Architecture

- **Bronze:** raw ingested tables (synthetic data extracts)

- **Silver:** typed + cleaned + derived metrics (sessions present, absence flags, bands)

- **Gold:** curated dimensions/facts optimised for Power BI semantic models



### Screenshots

See `/screenshots` for report pages, model diagram, and Fabric medallion tables.

- https://github.com/mike-analyticstudio/SEND-and-Education-Demo/tree/main/Screenshots\Dashboard : 
Various dashboards of the Executive Overview, Fundings, Pupil Level, School metrics and analytics 

- https://github.com/mike-analyticstudio/SEND-and-Education-Demo/tree/main/Screenshots/Data
Overview of raw source data

- https://github.com/mike-analyticstudio/SEND-and-Education-Demo/tree/main/Screenshots\Notebook
Overview of the spark notebook which handles the csv source files, right up to the implementation of the Medallion Architecture build the final 'Star' schema model presented to analytics tools

- https://github.com/mike-analyticstudio/SEND-and-Education-Demo/tree/main/Screenshots\Semantic Model
Overview of modelling of the dimensions and facts in a star schema

- https://github.com/mike-analyticstudio/SEND-and-Education-Demo/tree/main/Screenshots\Table Schema
Gold tier SQL_Lakehouse table schema for the bases of the analytics


Always interested in connecting with others working in:

- Public sector data platforms
- Education analytics
- SEND performance monitoring
- Impact measurement frameworks

- **Public Repo**: This repo is a Public repo that showcases Case study + screenshots + technical overviews

- **Private repo**: Full scripts, data, pipelines, templates, and other utility implementation available on request (client access)

#PowerBI #MicrosoftFabric #SEND #EducationAnalytics #BusinessIntelligence #DataEngineering #DfE #ImpactMeasurement

