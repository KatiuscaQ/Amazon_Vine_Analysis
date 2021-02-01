# Amazon_Vine_Analysis

![](https://github.com/KatiuscaQ/Amazon_Vine_Analysis/blob/main/Resources/amazon-vine-voices-adlucent.png)


## Overview of the analysis: 
Analyzed an Amazon dataset of Books Reviews by using PySpark to perform an ETL process to extract the data, transform it, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, use PySpark to determine if there is any bias toward favorable reviews from Vine members in the analyzed dataset. Then, write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.

*Dataset: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Books_v1_02.tsv.gz*

## Results: 

### o	How many Vine reviews and non-Vine reviews were there?

After filtering the data in total votes that were equal or greater than 20, and in helpful votes were the result of helpful votes and total votes were equal or greater than 50%, the count of “Vine reviews” and “Non-vine reviews” are as follow:

`Vine reviews: 0 `

`Non-Vine reviews: 403807`

### o	How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

Based on the previous results the 5-star vine reviews were again 0 (zero), meanwhile the non-vine 5-star reviews were 242889.

### o	What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

The percentage of 5-star vine reviews is again 0, and the percentage of 5-star non-vine reviews was around 60%


## Summary: 

Base on the results obtained there is no information to state if there is bias for the reviews coming from the Vine Program, there is no enough reviews considered valuable that came from the Vine Program.

Below a screenshot of the analysis:

![](https://github.com/KatiuscaQ/Amazon_Vine_Analysis/blob/main/Resources/count_of_vine_and_nonvine.PNG)

## Additional Analysis

An additional analysis performed on this dataset was to compare the results of non-vine reviews (unpaid_reviews) that were made by verified purchases and unverified purchases. Does purchase verification affect this specific dataset?

Also, the ratings in between the two newly analyzed sub-groups were compared. Following are the results:
The image below shows a screenshot of the results of how many verified purchases are giving ratings and how many unverified ones are doing the same and the percentage of each one:

![](https://github.com/KatiuscaQ/Amazon_Vine_Analysis/blob/main/Resources/verified_vs_unverified.PNG)

The image below shows a dataframe comparing the amount of “stars” given from verified purchases and unverified purchases:

![](https://github.com/KatiuscaQ/Amazon_Vine_Analysis/blob/main/Resources/rating_vs_purchaseverification.PNG)

The ratings coming from the unverified purchases are around 88% in comparison with the verified purchases.
91% of 1 star rating came from unverified purchases.
87% of 2 stars rating came from unverified purchases.
85% of 3 stars rating came from unverified purchases.
87% of 4 stars rating came from unverified purchases.
88% of 5 stars rating came from unverified purchases.





