# Amazon_Vine_Analysis

## Project Overview

The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. We will analyze Amazon reviews written by members of the paid Amazon Vine program to determine if having a paid Vine review makes a difference in the percentage of 5-star reviews.

## Tools Used
Use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Then use PySpark and Pandas to determine if there is any bias toward favorable reviews from Vine members in the dataset.

### Deliverable 1: Perform ETL on Amazon Product Reviews:
View the ETL Process in a Google Colaboraty Notebook Here

### Deliverable 2: Determine Bias of Vine Reviews
View the Vine Reviews Bias Analysis Here

## Results

How many Vine reviews and non-Vine reviews were there?

![vine vs non-vine] (https://github.com/pnimma01/Amazon_Vine_Analysis/blob/f1ac17ee13ae24c780c8a12772d0e3c5128058b2/Resources/D2/D2_Review_Counts.png)

1,266 Vine Reviews
62,004 Non_Vine Reviews

How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

![5 star vine_non_vine] (https://github.com/pnimma01/Amazon_Vine_Analysis/blob/f1ac17ee13ae24c780c8a12772d0e3c5128058b2/Resources/D2/D2_5_Star_Reviews.png)

432 Vine Reviews were 5 Stars
29,965 Non_Vine Reviews were 5 Stars


What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

![5 star Percent] (https://github.com/pnimma01/Amazon_Vine_Analysis/blob/f1ac17ee13ae24c780c8a12772d0e3c5128058b2/Resources/D2/Percent_5_Star.png)

34.12% of Vinew Reviews were 5 Stars.
48.32% of Non-Vine Reviews were 5 Stars.


## Summary

Is there is any positivity bias for reviews in the Vine program?

The results above for this specific dataset prove that there is no positivity bias towards 5 star reviews when comparing Vine reviews versus Non-Paid for by Vine Reviews.
The percent of reviews that were not paid for by Vine, had a higher percentage of 5 star ratings than those that were paid for by the Vine program. Only 34.12% of Vinew Reviews were 5 Stars while 48.32% of Non-Vine Reviews were 5 Stars.

### Additional Analysis

Additional analysis that we could do with the dataset would be to compare all star reviews (from 0 to 5) across paid for and unpaid for reviews as well as calculate and compare the average star rating for Vine and non-Vine reviews.