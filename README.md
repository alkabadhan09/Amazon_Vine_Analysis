# Amazon_Vine_Analysis

## Overview

Since ur work with Jennifer on SellBy project was so successful, we've been tasked with a larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

We had have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. I picked the dataset pertaining to the 'outdoors' and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I used Pandas to determine if there is any bias toward favorable reviews from Vine members in your dataset.


## Results

![amazon_vine](https://user-images.githubusercontent.com/107225715/201244227-b55061b8-9407-4455-914c-e2fe1529b2bc.png)

* How many Vine reviews and non-Vine reviews were there?


There are 107 Vine reviews and 39869 non-Vine reviews.

* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?


5 star Vine reviews - 56

5 star non-Vine reviews - 21005

* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?


% of 5 star Vine reviews - 52.34%

% of 5 star non-Vine reviews - 52.69%


## Summary

There is a positivity bias in the reviews for the Vine program. The volume of 5 star non-Vine reviews are very close to percentage of the 5 star Vine reviews. With a 52.69% 5 star review total versus 52.34% both the Vine & non-Vine reviewers are enjoying the program. 

Additional analysis that we can provide would be to utilize the 1 star to 4 star reviews as well as finding the mean, mode, mediun and STD seperately and between the two.
