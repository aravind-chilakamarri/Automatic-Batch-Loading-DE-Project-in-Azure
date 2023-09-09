# Automatic-Batch-Loading-DE-Project-in-Azure
It is a Automatic Batch loading Data Engineering Project which uses the medallion architecture for transforming the data from RAW format to the most curated format and creating the data analysis report for the end users.

PS: I have written rough notes of my implementation and asked ChatGPT to create technical documentations from them.<br />

## On-Premises:<br />
SQL Server<br />
Microsoft SQL Server Studio<br />
AdventureWorksLT Database (downloaded online)<br />
PowerBI desktop<br />

## AZURE SERVICES USED:<br />

### Azure Data Factory:<br />
To create a connection from on-premises and run the DATA INGESTION activity from SQL Server to Azure containers.<br />
### Azure DataLake Gen2:<br /> 
To store raw data (staging layer) and transformed data.<br />
### Azure Databricks:<br />
To do Data Transformations using raw data and reload them into Azure Datalake Gen2 (integration and access layers)<br />
### Azure Synapse:<br />
To run the SQL queries on top of datalake containers and load them into Azure SQL Server.<br />
Azure KeyVault: store sensitive information like usernames, passwords and access tokens<br />

