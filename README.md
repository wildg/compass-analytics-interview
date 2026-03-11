# compass-analytics-interview

<i>
You are building a customer 360º model for a sports and entertainment company to support the various business units in their decision making and tactical efforts. The data engineering team has already ingested various data sources into the bronze and silver layers and has made their data tables available for you to build their data model.

<br>

The primary objective is to build a customer 360 data model that can support various customer analytics use cases from: customer lifetime value, customer segmentation, customer churn, customer targeting & retention, prospective premium customers, willingness to pay, etc.
</i>

> **360 Degree Models** <br>
> Data modeling strategy that integrates every available data point about a specific entity into a single, unified view. In the context of this case, the entity in question is a customer

## Datasets
| SOURCE SYSTEM | DATASET |
|---------------|---------|
| Ticketmaster | - `ticket_purchases.csv`: Online ticket purchases per event <br> - `event_attendance.csv`: Attendance scan-ins by customers <br> - `events.csv`: Metadata for each event |
| Salesforce CRM | - `crm_interactions.csv`: Contact history and opportunity stages |
| Google Analytics | - `web_sessions.csv`: Website sessions including source, duration, and engagement |
| Retail POS | - `retail_transactions.csv`: In-venue or merchandise store purchases |
| Customer Profiles | - `customer.csv`: Partial demographic and signup metadata across systems |
| Customer Linkage | - `customer_linkage.csv`: A mapping table linking system-specific customer IDs to a shared universal_id |

## Task #1: Identify Resolution Strategy
<i>
The linking table was developed by a previous internal employee and may have errors thus the client has hired us to provide a new identity resolution strategy to unify the source systems. Your task is to describe (in a diagram, slide and/or pseudocode) how you would approach doing identity resolution across their many systems based on your expertise. Note that a linkage table is provided in the datasets .zip will be used for task #3 while your goal here is to design and not to implement.
</i>

<br>

> **Assumptions** <br>
> - TODO

## Task #2: Build the Customer 360 Gold Table
<i>
Using the datasets provided, as well as the linkage table, design and implement a consolidated customer_360 table. The table should also include the following features (or as many as are feasible). Implement this in a Jupyter Notebook (or an equivalent platform).

<br>

- Total ticket spend (lifetime)
- Number of unique events attended
- Average ticket value
- Total merchandise/retail spend
- Number of retail purchases in the last 90 days
- Days since last brand interaction (via any channel: ticket, web, retail, or CRM)
</i>

> **Assumptions**
> - TODO

## Task #3: Data Platform Overview
<i>
The client’s systems are based on legacy RDBMS data mart with pipelines stitched together with cron jobs running on virtual machine (VMs) while data governance is non-existent except for tribal knowledge accumulated within the IT team. Your task is to propose (as a diagram or a slide) a high-level data platform architecture to host the pipelines integrating source data to a centralized repository, and which is cloud-native, scalable, and can do both Data & ML. You may combine multiple platforms and tools as long as you can explain what and why to the client.
</i>

<br>

> **Assumptions**
> - TODO

<!--
Ideas:
- Provide different options for the data platform using different platforms (i.e. AWS, Azure, Google Cloud, Databricks, Dataiku, Snowflake). Base the suggestions on specific situations
- Identify specific ways to pull from different data sources. Create a new slide for each of the data sources
- Identify which flows need to be migrated and how they should be migrated
-->

## Project Extensions

> **Assumptions**
> - **Canadian Law**: The project is for a Canadian business. Thus, we only have to worry about Canadian regulation

### Data Governance
<!-- Consider performing governance training on best practices for the data platform -->
TODO

### IT & Business Continuity
<!-- Establish a plan to maintain the data pipeline and migration knowledge and keep teams un-siloed -->
TODO

### Regulatory Compliance
<!-- Consider any regulatory issues with the data -->
TODO

### Future State
<!-- Recommend future state changes to make the data pipeline better and suggest potential upgrades to the system. Include additional external data sources and how they should be pulled -->
TODO