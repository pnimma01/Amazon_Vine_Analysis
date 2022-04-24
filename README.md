** I worked with Aman Gill for this project, we follwed pair programming.

# Amazon_Vine_Analysis

## Project Overview

The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. We will analyze Amazon reviews written by members of the paid Amazon Vine program to determine if having a paid Vine review makes a difference in the percentage of 5-star reviews.

## Tools Used
Use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Then use PySpark and Pandas to determine if there is any bias toward favorable reviews from Vine members in the dataset.

### Deliverable 1: Perform ETL on Amazon Product Reviews:
View the ETL Process in a Google Colaboraty Notebook [here](https://github.com/pnimma01/Amazon_Vine_Analysis/blob/c71df21e34617c73add139a799fa1b61af4bc87a/Amazon_Reviews_ETL.ipynb)

### Deliverable 2: Determine Bias of Vine Reviews
View the Vine Reviews Bias Analysis [here](https://github.com/pnimma01/Amazon_Vine_Analysis/blob/c71df21e34617c73add139a799fa1b61af4bc87a/Vine_Review_Analysis.ipynb)

## Results

How many Vine reviews and non-Vine reviews were there?

![vine vs non-vine](https://github.com/pnimma01/Amazon_Vine_Analysis/blob/f1ac17ee13ae24c780c8a12772d0e3c5128058b2/Resources/D2/D2_Review_Counts.png)

1,266 Vine Reviews

62,004 Non_Vine Reviews

How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

![5 star vine_non_vine](https://github.com/pnimma01/Amazon_Vine_Analysis/blob/f1ac17ee13ae24c780c8a12772d0e3c5128058b2/Resources/D2/D2_5_Star_Reviews.png)

432 Vine Reviews were 5 Stars

29,965 Non_Vine Reviews were 5 Stars


What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

![5 star Percent](https://github.com/pnimma01/Amazon_Vine_Analysis/blob/f1ac17ee13ae24c780c8a12772d0e3c5128058b2/Resources/D2/Percent_5_Star.png)

34.12% of Vinew Reviews were 5 Stars.

48.32% of Non-Vine Reviews were 5 Stars.


## Summary

Is there is any positivity bias for reviews in the Vine program?

No, there is no positivity bias in the Vine program, based on the results.

## Additional Analysis

Following additional analysis can be performed on the data:
- Compare all the reviews (0 to 5 stars) across paid for and unpaid.
- Calculate and compare the average star rating for Vine and non-Vine reviews.