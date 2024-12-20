# Home_Sales

## Setup

This project utilized Google Colab. The very first cell is important as this is what sets up our environment to run Spark and Java. 

Google Colab also requires an account, so if you do not have one, you will have to replicate the environment on your own.


## Analysis

For this project, we analyzed Home Sales from 2010 to 2017. We analyzed the average prices of different types of homes in different ways. 

1. First, we loaded the data into a spark view directly from a csv. We then ran a handful of queries to analyze the time taken to execute.
2. We then cached the temp view and reran one of the queries and analyzed the execution time.
3. Finally, we partitioned the data by the ```date_built``` column. We then saved the dataset in a parquet format. We then read this back into a view, and executed the same query as in step 2 to analyze the execution time.