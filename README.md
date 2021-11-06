# Amazon_Vine_Analysis

![Amazon](https://www.ecomengine.com/hubfs/images/featured/blog/amazon-vine-program-for-sellers.jpg)

###### Source: *https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt*

## Overview of the analysis

The main purpose of this analysis is performing an ETL process to extract a dataset, transform this data, connect to an Amazon Web Services RDS instance and load that transformed data into PgAdmin. With this in mind we can analyze and determine if exist and favorable reviews from Vine memmers in order to give a exact analysis.

## Results:

There is a total of 4,291 vine member reviews while there is 1,781,706 non vine members. This is considering only vine or non vine members as filters.

There is a total of 4,291 vine member reviews while there is 1,781,706 non vine members. This is considering only vine or non vine members as filters, as you can see in the following images:

![TotalVineMembers](https://github.com/alesandelmoral/Amazon_Vine_Analysis/blob/main/Images/TotalVineMembers.PNG)

![TotalNOVineMembers](https://github.com/alesandelmoral/Amazon_Vine_Analysis/blob/main/Images/TotalNOVineMembers.PNG)

Analyzing all the filters to retrieve each the rows with the total votes count equal or greater than 20 and filtering the data again in order to get all the rows where the helpful votes are divided by the total votes in the respective columns that are equal or greater than 50%. There were a total of 94 votes that were paid and only 48 of those votes were 5 stars making it only 51.06%, again, the total was obtained considering the previously filters mentioned above. The total votes of the unpaid ones is 40,471, but only 15,663 of the total voted for a 5 star, making 38.70% of the unpaid votes.

![Analysis_1](https://github.com/alesandelmoral/Amazon_Vine_Analysis/blob/main/Images/Analysis_1.PNG)

![Analysis_2](https://github.com/alesandelmoral/Amazon_Vine_Analysis/blob/main/Images/Analysis_2.PNG)

In order to verify the purchase of the product we made a double check filter, it shows that non of the vine members purchased the products and gave a 5 star, while 3,862 of 10,106 unpaid ones gave a 5 star rate covering a 38.21% of the verified purchase 5 star rate for the unpaid members.

![Double_filter](https://github.com/alesandelmoral/Amazon_Vine_Analysis/blob/main/Images/DoubleFilter1.PNG)


## Summary

Througth the analysis we can see from the results that don't any positivity bias for the reviews in the vine program, even if the votes are from a verified purchase, and even if considering the unverified purchase, it might be a lot 51.06% but at the same time, that considers low voters count in comparison with the non paid members. 
With the last validation that we did help us to see the difference as accurate as possible so that it becomes a deeper analysis that the one that we have at the beginning.



