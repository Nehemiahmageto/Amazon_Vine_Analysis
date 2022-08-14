# Amazon_Vine_Analysis

## Overview of the analysis of the Vine program

Using PySpark, this project will analyze Amazon reviews from members registered in the Amazon Vine program. Some companies pay a fee to Amazon that allow them to provide free products to Vine members who in turn publish reviews. This service also allows us to determine whether there is any bias towards favorable reviews from Vine members vs. non-members.

For this project, I analyzed reviews under the "Video Games" category as it has been a progressive market since the pandemic.

## Results

To reduce the dataframe and get the most helpful reviews, I extracted reviews with total votes greater than or equal to 20.

![alt text](https://github.com/Nehemiahmageto/Amazon_Vine_Analysis/blob/main/images/capture.png)

Next was to extract the helpful votes using the criteria of helpful votes / total votes being greater than 50%.

![alt text](https://github.com/Nehemiahmageto/Amazon_Vine_Analysis/blob/main/images/capture2.png)

The dataframe was then split according to vine program reviews and non vine program reviews.

![alt text](https://github.com/Nehemiahmageto/Amazon_Vine_Analysis/blob/main/images/capture3.png)

![alt text](https://github.com/Nehemiahmageto/Amazon_Vine_Analysis/blob/main/images/capture4.png)

The results were as below:

![alt text](https://github.com/Nehemiahmageto/Amazon_Vine_Analysis/blob/main/images/capture5.png)

1. Total number of Vine and non-Vine reviews
* 94 vine reviews
* 40,471 non-vine reviews

2. Total number of 5 star Vine reviews and non-Vine reviews
* 48 5 star Vine reviews
* 15,663 5 star non-Vine reviews

3. Percentage of 5 star Vine reviews and on-Vine reviews
* 51.06% 5 star Vine reviews
* 38.70% 5 star non-Vine reviews

## Summary
We can conclude that there is a positivity bias for reviews in the Vine program since there is a large difference in 5 star review percentage of 12.36%(51.06-38.70). Vine customers are more prone to 5 star reviews even when the product is not s good.

For a much more clear review of bias in the reviews, we should use all the data, even those with a low total vote count and perhaps check for bias in a number of products.
