# Amazon Vine Analysis

## Overview of the analysis: 
Using your knowledge of the cloud ETL process, you’ll create an AWS RDS database with tables in pgAdmin, pick a dataset from the Amazon Review datasets, and extract the dataset into a DataFrame. You'll transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Then, you'll upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.
You’ll use PySpark to determine if there is any bias toward favorable reviews from Vine members in your dataset. 

## Results: 

### - How many Vine reviews and non-Vine reviews were there?
There were 162 total Vine reviews and 35,606 total non-Vine reviews.
Image of DataFrame with all the the review data for non-Vine reviews:
<img width="650" alt="Screen Shot 2022-08-22 at 12 56 48 PM" src="https://user-images.githubusercontent.com/103215686/185997721-a90a5d0a-a6bf-48f8-8581-b700cba2efc9.png">

### - How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
There were 63 5 star Vine reviews and 19,444 5 star non-Vine reviews.

Image of DataFrame for all Vine review data and the PySpark code to determine total reviews and 5 star reviews:
<img width="444" alt="Screen Shot 2022-08-22 at 12 59 55 PM" src="https://user-images.githubusercontent.com/103215686/185998335-dba8619d-9d44-46fb-8c03-9ea45072c28c.png">

<img width="412" alt="Screen Shot 2022-08-22 at 12 59 37 PM" src="https://user-images.githubusercontent.com/103215686/185998603-d305adb8-53e9-42fc-8069-943037c5d1db.png">

### - What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
39% of Vine reviews were 5 stars. 55% of non-Vine reviews were 5 stars.


## Summary: 
After analyzing the results, there is no positivity bias in the Vine program. Only 38% of reviews were 5 stars, which is an accepted amount. 
One additional analysis that we could complete with this dataset is compare which products got the highest reviews and if they were consistent between the Vine and non-Vine programs.
