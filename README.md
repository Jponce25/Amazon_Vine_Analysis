# Amazon_Vine_Analysis

## Overview of the analysis
We have been tasked to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, we pick one of these datasets and use PySpark to perform the cloud ETL process to extract the dataset, transform the data, also we create an AWS RDS database with tables in pgAdmin, and load the transformed data into pgAdmin. Next, we use PySpark to determine if there is any bias toward favorable reviews from Vine members in your dataset.

## Results

<img src="https://github.com/Jponce25/Amazon_Vine_Analysis/blob/9b425481f86f9d0b30cd24ff51ae078cfe217b90/Image/Imagen1.png" width="700">
<img src="https://github.com/Jponce25/Amazon_Vine_Analysis/blob/9b425481f86f9d0b30cd24ff51ae078cfe217b90/Image/Imagen3.png" width="700">

**• How many Vine reviews and non-Vine reviews were there?**

Number of reviews for paid Vine program was: 94

Number of reviews for unpaid Vine program was: 40471

**• How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**

Number of 5-star reviews for paid Vine program was: 48

Number of 5-star reviews for unpaid Vine program was: 15663

**• What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**

Percentage of 5-star reviews for paid Vine program was: 51.06%

Percentage of 5-star reviews for unpaid Vine program was: 38.70%

## Summary

<img src="https://github.com/Jponce25/Amazon_Vine_Analysis/blob/9b425481f86f9d0b30cd24ff51ae078cfe217b90/Image/Imagen2.png" width="600">
<img src="https://github.com/Jponce25/Amazon_Vine_Analysis/blob/9b425481f86f9d0b30cd24ff51ae078cfe217b90/Image/Imagen4.png" width="600">

A positive deviation in the reviews of the Vine program is observed, since more than half of the paid reviews (51.06%) resulted in 5 stars, while of the total unpaid reviews only 38.70% resulted in 5 stars.

An additional analysis could be to include the verified_purchase variable to identify if a greater number of stars is accompanied by a verified purchase.