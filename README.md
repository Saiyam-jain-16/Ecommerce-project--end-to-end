A data engineering project on Databricks that takes raw e-commerce CSV files, cleans them with PySpark, and organizes them into Bronze, Silver, and Gold Delta tables that are ready for SQL analysis.

Overview

Raw e-commerce data is messy: duplicates, missing values, wrong data types, stray symbols, and typos. This project builds a Medallion pipeline on Databricks that fixes these problems step by step and ends with a clean star schema that answers business questions about revenue, products, channels, and customers.




