## Home_Sales
**Module 22 Challenge - Big Data**

In this scenario, I used my knowledge of SparkSQL to determine key metrics about home sales data. I used Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table had been uncached. I used Google Colab to write and run my code.

**The url to resource file:**

https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.2/22-big-data/home_sales_revised.csv


**Repository Contents:**
- Home_Sales.ipynb

## Table of Contents

- [About](#about)
- [Getting Started](#getting-started)
- [Installing](#installing)
- [Contributing](#contributing)



## About

### I ran queries to answer the following questions:

#### - What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
  
![image](https://github.com/KTamas03/Home_Sales/assets/132874272/5f5442fa-da98-4e9c-babd-065fe2711822)

#### - What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

![image](https://github.com/KTamas03/Home_Sales/assets/132874272/cedcfa9d-538a-4c70-aafc-a657dd2f3525)


#### - What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

![image](https://github.com/KTamas03/Home_Sales/assets/132874272/df92c0d7-0a43-4a86-9f8f-ae43b60fa5ed)


 #### - What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

##### Uncached Data:

Took approximately 1.54 seconds for the query because each query required reading the data from storage, resulting in longer input/output time.
    
   ![image](https://github.com/KTamas03/Home_Sales/assets/132874272/6d5d9eff-6e2c-4487-99e5-554c908d2954)

##### Cached Data:

Significantly improved performance on uncached data, reducing the query time to around 0.47 seconds. This is because the data was stored in memory, allowing for faster query execution directly from memory.
    
   ![image](https://github.com/KTamas03/Home_Sales/assets/132874272/9057486a-51a4-40ca-bf85-264f8037ef05)

##### Parquet Data:

Fell between the uncached and cached versions, with a query time of about 0.93 seconds. The slight delay can be attributed to the need to access and process data from multiple partitions, introducing additional input/output and overhead.
    
   ![image](https://github.com/KTamas03/Home_Sales/assets/132874272/61d410a0-32a8-4b1a-8482-d060ec14bb89)


**Resource Files I Used:**
  - home_sales_revised.csv

**Partitioned_data:**

![image](https://github.com/KTamas03/Home_Sales/assets/132874272/21e32ceb-24ed-4152-9212-9d4774646435)



**My Python Script:**
  - Home_Sales.ipynb

**Tools/Libraries I Imported:**
   - import os: Used for interacting with the operating system, like setting environment variables or working with file paths.
   - import findspark: Used to locate and initialize a Spark installation in your Python environment, making it accessible for PySpark applications.
   - from pyspark.sql import SparkSession: Used to create a SparkSession, which is the entry point for using PySpark SQL functionality.
   - import time: Used for time-related functions, such as measuring execution time or introducing delays in code.
   - from pyspark import SparkFiles: Used for adding and accessing files to the Spark cluster, making external files available for Spark workers during data processing.


## Getting Started

**Programs/software I used:**
 - Google Colab: online tool that allows you to write and execute python in your browser.

## Installing
- Install Spark and Java (refer to first cell in Home_Sales.ipynb for code required to install)
  
