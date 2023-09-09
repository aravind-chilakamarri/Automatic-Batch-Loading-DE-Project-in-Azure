# Automatic-Batch-Loading-DE-Project-in-Azure
It is a Automatic Batch loading Data Engineering Project which uses the medallion architecture for transforming the data from RAW format to the most curated format and creating the data analysis report for the end users.

PS: I have written rough notes of my implementation and asked ChatGPT to create technical documentations from them.

On-Premises:
SQL Server
Microsoft SQL Server Studio
AdventureWorksLT Database (downloaded online)
PowerBI desktop

AZURE SERVICES USED:

Azure Data Factory: To create a connection from on-premises and run the DATA INGESTION activity from SQL Server to Azure containers.
Azure DataLake Gen2: To store raw data (staging layer) and transformed data.
Azure Databricks: To do Data Transformations using raw data and reload them into Azure Datalake Gen2 (integration and access layers)
Azure Synapse: To run the SQL queries on top of datalake containers and load them into Azure SQL Server.
Azure KeyVault: store sensitive information like usernames, passwords and access tokens

