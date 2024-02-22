---
{"dg-publish":true,"permalink":"/digital-brain/050-data-analytics/data-warehouse/"}
---

A data warehouse is a single source of truth. It contains all the data of a company. It is a source of information. The features of the data warehouse are:
1. Non Volatile: meaning data once stored will not go away.
2. Summarized: The data is processed, segmented and stored so that analytics tool can use them
3. Time Variant: It  stores data for a period of time. It also contains historical data.
4. Integrated: It has work with various analytics and reporting tools.
5. Subject Oriented: Its stores data related to a subject.

Base = CRM, GA
Secondary = repository like Looker to aggregate the data for reporting 

Tier 1 = Looker 

Tier 2 = separation on raw data from reporting data. Cleaning up and enriching the data before reporting
Disadvantage = pipeline complexity if a lot of data sources

Tier 3 = specialized tools for all process

[[Digital Brain/050 Data Analytics/050 Data Analytics MOC\|050 Data Analytics MOC]]