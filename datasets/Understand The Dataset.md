## Overview
  The data provided for the GSynergy project is retail or sales-related data, structured for data warehousing and analytics.
  It includes fact tables (transactional data) and dimension tables (hierarchical data), which are typical components of a star schema.
  This data can be used for sales analysis, inventory management, cost analysis, and more.


#### The Dataset is present in Azure Storage Account which contains 10 delimited files as follows:
  Fact Tables:
  	•	fact.averagecosts.dlm.gz 
    •	fact.transactions.dlm.gz
  
  Dimension (Hier) Tables:
  	•	hier.clnd.dlm.gz (Calendar)
  	•	hier.hldy.dlm.gz (Holiday)
  	•	hier.invloc.dlm.gz (Inventory Location)
  	•	hier.invstatus.dlm.gz (Inventory Status)
  	•	hier.possite.dlm.gz (POS Site)
  	•	hier.pricestate.dlm.gz (Price State)
  	•	hier.prod.dlm.gz (Product)
  	•	hier.rttloc.dlm.gz (Retail Location)

   
1. **Bronze Layer**: Stores raw data as-is from the source systems(Azure Storage). Data is ingested from DML Files into AzureSQL Database.
2. **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.

1. **Bronze Layer**: Stores raw data as-is from the source systems(Azure Storage). Data is ingested from DML Files into AzureSQL Database.
2. **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.



#### This data can be used for:
  Sales Analysis:
  Analyze sales trends by product, store, region, or time period.
  Identify top-selling products or regions.
  Inventory Management:
  Track inventory status and location.
  Optimize stock levels based on sales trends.
  Cost Analysis:
  Analyze the impact of product costs on profitability.
  Holiday Sales Analysis:
  Compare sales performance during holidays vs. non-holidays.
  Channel Performance:
  Analyze sales performance by channel (e.g., online, in-store).
