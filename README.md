# Home_Sales

This project involves analyzing home sales data using PySpark, performing SQL queries, and optimizing performance through caching and partitioning. The goal is to process, query, and analyze home sales data efficiently and draw insights using Spark's capabilities.

# Project Steps

1. Rename Notebook: Rename Home_Sales_starter_code.ipynb to Home_Sales.ipynb.

2. Import Libraries: Import necessary PySpark functions for data processing and SQL queries.

3. Load the Dataset: Read the home_sales_revised.csv file into a PySpark DataFrame.

4. Create Temporary Table: Create a temporary table named home_sales from the DataFrame for running SQL queries.

# Analysis Questions

Using SparkSQL, answer the following queries:

1. Average Price of Four-Bedroom Houses by Year:

    * Compute the average price of four-bedroom houses sold for each year. Round results to two decimal places.

2. Average Price for Homes with Three Bedrooms and Three Bathrooms by Year Built:

    * Calculate the average price of homes with three bedrooms and three bathrooms for each year they were built, rounding to two decimal places.

3. Average Price for Homes with Specific Features:

    * Determine the average price for homes with three bedrooms, three bathrooms, two floors, and at least 2,000 square feet, grouped by the year built.

4. Average Price by "View" Rating:

    * Compute the average home price for each "view" rating where the average home price is at least $350,000. Measure the runtime and round the results to two decimal places.

# Optimization Steps

1. Cache the Temporary Table: Cache the `home_sales` table to improve query performance.

2. Verify Caching: Check if the table is cached successfully.

3. Re-run the Query Using Cached Data: Run the query for the average price per "view" rating using the cached data and compare the runtime with the uncached version.

4. Partition Data by "Date Built": Partition the home sales data by the `date_built` field, saving the output as a Parquet file.

5. Create a Temporary Table for Partitioned Data: Create a temporary table from the partitioned Parquet file.

6. Run the "View" Rating Query on Partitioned Data: Re-run the query on the partitioned data and compare the runtime with the uncached version.

# Final Steps

1. Uncache the Table: Uncache the `home_sales` table to free up memory.

2. Verify Uncaching: Ensure the table has been successfully uncached.

3. Upload to GitHub: Download the final `Home_Sales.ipynb` file and upload it to your "Home_Sales" GitHub repository.

# Technologies Used

* PySpark: For large-scale data processing.
* SparkSQL: For querying the data using SQL syntax.
* Parquet: For efficient data storage and partitioning.




__Author__: Adriel Garcia

__How to Run__

* Install necessary dependencies (PySpark)
* Upload `Home_Sales_colab.ipynb` to Colab
* Load the home_sales_revised.csv dataset.
* Run each section of the notebook step-by-step to perform the analysis and optimization.