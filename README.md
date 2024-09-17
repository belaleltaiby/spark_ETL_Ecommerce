# Ecommerce_ETL_Spark
1) Data Ingestion: Load data from HDFS for spark processing.
2) Data Processing and Transformation:
  **Using RDDs:**
    - Perform a transformation to filter out any corrupted or incomplete records from the 
      transaction data.
    - Implement a custom transformation to anonymize user IDs for privacy compliance.
  **Using DataFrames:**
    - Clean and standardize inventory data (e.g., handling missing values, normalizing text).
    - Join user activity logs with transaction records to analyze user behavior leading to 
      purchases.
  **Using Spark SQL:**
    - Create temporary views and execute SQL queries to compute:
    - Top 10 most purchased products in the last month.
    - Monthly revenue trends.
    - Inventory turnover rates.
  
3)Data Storage: Using Parquet format for batch-processed data in HDFS.
4)Performance Optimization:
   - Caching DataFrames to optimize performance for multiple transformations
   - Repartition DataFrames for optimal join performance.
   - Use Broadcast Join for small DataFrames

5)Sample Dashboard Outputs:
   - **Top Products Bar Chart:** Displaying the top 10 products with the highest sales.
   - **Revenue Trend Line Chart:** Showing monthly revenue over the past year.
