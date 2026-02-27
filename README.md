## SEND \& Education Analytics Platform (Hybrid LA + MAT)



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

- \Screenshots\Dashboard : 
Various dashboards of the Executive Overview, Fundings, Pupil Level, School metrics and analytics 

- \Screenshots\Data

- \Screenshots\Notebook
Overview of the spark notebook which handles the csv source files, right up to the implementation of the Medallion Architecture build the final 'Star' schema model presented to analytics tools

- \Screenshots\Semantic Model
Overview of modelling of the dimensions and facts in a star schema

- \Screenshots\Table Schema
Gold tier SQL_Lakehouse table schema for the bases of the analytics

- **Public Repo**: This repo is a Public repo that showcases Case study + screenshots + technical overviews

- **Private repo**: Full scripts, data, pipelines, templates, and other utility implementation available on request (client access)

