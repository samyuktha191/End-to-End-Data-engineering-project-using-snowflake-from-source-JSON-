# End-to-End-Data-engineering-project-using-snowflake-from-source-JSON
Building a end to end DWH solution using snowflake

Project Name- Data engineering using snowflake

Overview:
This project aims to build an end-to-end data engineering pipeline using a sample cricket dataset. The pipeline includes loading data from JSON files into Snowflake, cleansing the unstructured data to convert it into a structured format, performing necessary transformations, and constructing a data warehouse (DWH) solution.

This use case involves utilizing Snowflake's free trial edition without employing external named stages or dependencies such as AWS or Azure. The focus is purely on the Snowflake instance itself, ensuring simplicity and ease of implementation.

Objective: This use case focuses on loading a JSON file into Snowflake using the Snowsite web UI and CLI, processing the data internally, and mimicking the functionality of an external named stage. We will follow a series of steps to profile, analyze, flatten, cleanse, and consume the data, culminating in the creation of BI dashboards.


Implementation Steps -
=>Load JSON File into Internal Named Stages
==>>Data Profiling and Root Level JSON Data Analysis
===>>>Storing Data, JSON Flattening, and Further Analysis
===>>>>Data Cleansing and Filtering Bad Records
===>>>>>Consumption Layer Development (Fact and Dimension Tables)
===>>>>>>BI/Dashboard Integration
===>>>>>>>Ongoing Data Ingestion and Automated Dashboard Refresh


Project Prerequisites
Snowflake Editions:
===>>Free Trial Edition
Tools:
===>>VSCode
===>>JSON File Visualizer (any free tool)
===>>DBeaver for data modeling
Data Loading:
===>>Snowsight Data Loading feature
Data Cleaning & Transformation:
===>>Snowsight Worksheet using SQL statements
Visualization:
===>>Snowsight Dashboard

Architecture in Snowflake
In Snowflake (or any DWH system), we follow a layered architecture with logically named layers:

Landing Layer
Description: Initial staging area for data.
Components: Named Stage, file formats.

RAW Layer
Description: Raw, unprocessed data.
Components: Flattened JSON data and metadata, data analysis, and profiling.

Clean Layer
Description: Processed data with logical entities.
Components: Flattened nested JSON data, creation of logical entities, and a cleaner dataset.

Consumption Layer
Description: Final, meaningful, and usable data.
Components: Data prepared for use, views for dashboards.

BI Layer
Description: Visualization and reporting.
Components: Snowsight filters and dashboards.



Data Modeling to build Cricket Datawarehouse Facts and Dimensions models. 


![cricket - CRICKET - CONSUMPTION](https://github.com/user-attachments/assets/d9031d2e-0003-48c9-a955-28698f03865c)

