## Home_Sales
**Module 22 Challenge - Big Data**

In this scenario, I used my knowledge of SparkSQL to determine key metrics about home sales data. I used Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table had been uncached. 

**The url to resource file:**

https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.2/22-big-data/home_sales_revised.csv


**Repository Folders and Contents:**
- Home_Sales_colab.ipynb
- Home_Sales.ipynb

## Table of Contents

- [About](#about)
- [Getting Started](#getting-started)
- [Installing](#installing)
- [Contributing](#contributing)



## About
### Part 1: Clean and Append Data in Jupter Notebook

I ran queries to answer the following questions:
- What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
  
![image](https://github.com/KTamas03/Home_Sales/assets/132874272/5f5442fa-da98-4e9c-babd-065fe2711822)

- What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

![image](https://github.com/KTamas03/Home_Sales/assets/132874272/cedcfa9d-538a-4c70-aafc-a657dd2f3525)


- What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

![image](https://github.com/KTamas03/Home_Sales/assets/132874272/df92c0d7-0a43-4a86-9f8f-ae43b60fa5ed)


 -What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

    - Uncached:
    
   ![image](https://github.com/KTamas03/Home_Sales/assets/132874272/6d5d9eff-6e2c-4487-99e5-554c908d2954)
    
    - Cached:
    
   ![image](https://github.com/KTamas03/Home_Sales/assets/132874272/9057486a-51a4-40ca-bf85-264f8037ef05)
    
    - Parquet Data:
    
   ![image](https://github.com/KTamas03/Home_Sales/assets/132874272/61d410a0-32a8-4b1a-8482-d060ec14bb89)


**Resource Files I Used:**
  - home_sales_revised.csv

**Partitioned_data:**

![image](https://github.com/KTamas03/Home_Sales/assets/132874272/21e32ceb-24ed-4152-9212-9d4774646435)



**My Jupyter Notebook Python Cleaning Script:**
  - Home_Sales_colab.ipynb

**Tools/Libraries I Imported:**
   - import findspark
   - from pyspark.sql import SparkSession
   - import time
   - from pyspark import SparkFiles


## Getting Started

**Programs/software I used:**
 - Jupyter Notebook: python programming tool, was used for data manipulation and consolidation.

**To activate dev environment and open Jupyter Notebook:**
- Open Anaconda Prompt
- Activate dev environment, type 'conda activate dev'
- Navigate to the folder where repository is saved on local drive
- Open Jupyter Notebook, type 'Jupyter Notebook'

## Installing

- Install Spark and Java (add instructions here)
  
## Contributing

- ???

