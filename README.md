# Challenge_22
## Big Data
In this challenge, I created a Spark DataFrame from the Home_Sales dataset.
I created a temporary table from the original DataFrame, ran the following queries, and they returned the following:
* The average price, rounded to two decimal places, of a four-bedroom house sold each year.
* The median price, rounded to two decimal places, of a home with three bedrooms and three bathrooms for each year it was built.
* The average price of a house with three bedrooms, three bathrooms, two stories, and is greater than or equal to 2,000 square feet for each year it was built, rounded to two decimal places.
* The average price of a home by 'view' rating that has an average home price greater than or equal to $350,000, rounded to two decimal places. The result shows the execution time of this query, which was 0.76 seconds.

A cache memory of the 'home_sales' temporary table was created and validated.

The query for the average price of a home by 'view' rating is executed on the cached temporary table, and the execution time is calculated, which is 0.68 seconds.

A partition of the home sales dataset was created using the 'construction_date' field, and the data in Parquet format was read.

A temporary table of the Parquet data was created.

I re-ran the query for the average price of a home by 'view' rating on the Parquet temporary table, and the execution time was calculated.

Finally, the cache was cleared, and it was verified that the 'home_sales' temporary table was not stored in the cache.
