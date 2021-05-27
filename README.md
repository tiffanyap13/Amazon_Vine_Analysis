# Amazon Vine Analysis
## Purpose
This analysis is of Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
## Overview
In this project, I selected the dataset with reviews of shoes and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I used PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset. 

## Results

 - There were 27,009 total reviews, of which 22 were paid reviews (part of the Vine program) and 26,987 were non-paid reviews (not part of the Vine program).
 ![Review Count] (Total_Reviews.png)
 - There were 14,488 5-star Vine reviews, of which 13 were paid (Vine) 5-star reviews and 14,475 were non-paid (non-Vine) 5-star reviews.
 - The percentage of Vine reviews that were 5-stars is 59%. The percentage of non-Vine reviews that were 5 stars is 53.6%.
 ![% Vine Reviews] (5_Star.png)
 
## Summary
In summary, it was determined that there may be some positivity bias since the percentage of paid (Vine) 5-star reviews is 59%, which is higher than the larger population of non-paid 5-star reviews, which was 53.6%.
One additional analysis that could be done with the dataset is to calculate the reviews based on actual verified purchase.  The reason for looking into this section of the data is to see if actual paying customers reviewed their purchased product.
