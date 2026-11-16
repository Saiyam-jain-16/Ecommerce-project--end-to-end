A data engineering project on Databricks that takes raw e-commerce CSV files, cleans them with PySpark, and organizes them into Bronze, Silver, and Gold Delta tables that are ready for SQL analysis.

Overview

Raw e-commerce data is messy: duplicates, missing values, wrong data types, stray symbols, and typos. This project builds a Medallion pipeline on Databricks that fixes these problems step by step and ends with a clean star schema that answers business questions about revenue, products, channels, and customers.

Architecture

Add your architecture images here (legacy setup vs Databricks setup):

Legacy architecture Databricks architecture

Medallion layers
Layer	What it holds	What happens here
Bronze	Raw data	Raw CSV files from a Unity Catalog Volume are loaded into Delta tables
Silver	Cleaned data	PySpark removes duplicates and nulls, fixes data types, symbols, and typos
Gold	Analytics-ready data	Star-schema tables are built, with amounts converted to INR
What was built



