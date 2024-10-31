# home_sales

In this project, I leveraged my knowledge of SparkSQL to analyze key metrics in home sales data. I utilized Spark to create temporary views, partitioned the data for optimized performance, cached and uncached a temporary table, and confirmed that the table was successfully uncached.

Instructions
Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.
Import the necessary PySpark SQL functions for this assignment.
Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.
Create a temporary table called home_sales.
Cache your temporary table home_sales.
Check if your temporary table is cached.
Using the cached data, run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
Partition by the "date_built" field on the formatted parquet home sales data.
Create a temporary table for the parquet data.
Run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
Uncache the home_sales temporary table.
Verify that the home_sales temporary table is uncached using PySpark.
Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.

Answer the following questions using SparkSQL:


Question - What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

Answer:
+----+-------------+
|year|average_price|
+----+-------------+
|2022|  $296,363.88|
|2021|  $301,819.44|
|2020|  $298,353.78|
|2019|  $300,263.70|

Question - What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

Answer:
+----+-------------+
|year|average_price|
+----+-------------+
|2010|  $292,859.62|
|2011|  $291,117.47|
|2012|  $293,683.19|
|2013|  $295,962.27|
|2014|  $290,852.27|
|2015|  $288,770.30|
|2016|  $290,555.07|
|2017|  $292,676.79|
+----+-------------+

Question - What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

Answer:
+------+---------------+
| view | average_price |
+------+---------------+
|   99 | $1,061,201.42 |
|   98 | $1,053,739.33 |
|   97 | $1,129,040.15 |
|   96 | $1,017,815.92 |
|   95 | $1,054,325.60 |
|   94 | $1,033,536.20 |
|   93 | $1,026,006.06 |
|   92 |   $970,402.55 |
|   91 | $1,137,372.73 |
|   90 | $1,062,654.16 |
+------+---------------+
Only showing top 10 rows.
Execution time: 0.42646312713623047 seconds


Home_Sales
Overview
In this challenge, I have used my knowledge of SparkSQL to determine key metrics about home sales data. Then I used Spark to create temporary views, partition the data, cache and uncache a temporary table, and verified that the table has been uncached.

Instructions
Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.
Import the necessary PySpark SQL functions for this assignment.
Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.
Create a temporary table called home_sales.
Cache your temporary table home_sales.
Check if your temporary table is cached.
Using the cached data, run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
Partition by the "date_built" field on the formatted parquet home sales data.
Create a temporary table for the parquet data.
Run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
Uncache the home_sales temporary table.
Verify that the home_sales temporary table is uncached using PySpark.
Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.
Answer the following questions using SparkSQL: Mentioned above!

Requirements
A Spark DataFrame is created from the dataset. (5 points)
A temporary table of the original DataFrame is created. (10 points)
A query is written that returns the average price, rounded to two decimal places, for a four-bedroom house that was sold in each year. (5 points)
A query is written that returns the average price, rounded to two decimal places, of a home that has three bedrooms and three bathrooms for each year the home was built. (5 points)
A query is written that returns the average price of a home with three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet for each year the home was built rounded to two decimal places. (5 points)
A query is written that returns the average price of a home per "view" rating having an average home price greater than or equal to $350,000, rounded to two decimal places. (The output shows the run time for this query.) (10 points)
A cache of the temporary "home_sales" table is created and validated. (10 points)
The query from step 6 is run on the cached temporary table, and the run time is computed. (10 points)
A partition of the home sales dataset by the "date_built" field is created, and the formatted parquet data is read. (10 points)
A temporary table of the parquet data is created. (10 points)
The query from step 6 is run on the parquet temporary table, and the run time is computed. (10 points)
The "home_sales" temporary table is uncached and verified. (10 points)

References:
In completing this assignment, I referenced a variety of supplementary resources to clarify coding concepts and enhance my understanding of data analytics techniques. Due to limited availability of tutoring support during my work hours, I consulted platforms such as Google, YouTube, ChatGPT, and reputable data analytics sites like GeeksforGeeks, Kaggle, and Stack Overflow. I also utilized AI tools for coding assistance and guidance on specific coding challenges, which provided additional clarity and support for troubleshooting issues outside of standard support hours.

The code and analyses presented in this assignment are authored by me, with these external resources and AI tools used strictly for educational and guidance purposes. This disclosure is intended to provide transparency to the grading staff, ensuring they understand the context of my consultations with external resources and that my work reflects my independent efforts.


