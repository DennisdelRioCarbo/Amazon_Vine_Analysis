#Amazon Vine Program Analysis

## Overview: 
The purpose of this project is to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
We accessed a dataset from the Amazon Review Datasets that contains reviews of video games and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Then, we used PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset. The following is  the analysis for the SellBy stakeholders.

# Deliverable 1. 
**Queries for populated tables in PGAdmin.**

**customers_table**

![customers_table](https://user-images.githubusercontent.com/104289098/185771934-44e7283c-9bca-48b6-a1a6-a5744df2a008.png)

**products_table**

![products_table](https://user-images.githubusercontent.com/104289098/185771943-fed1d827-339f-4327-b98a-6d6e9fce4b27.png)

**review_id_table**

![review_id_table](https://user-images.githubusercontent.com/104289098/185771962-8a391542-d4a4-4450-8fed-567a27b9d8da.png)

**vine_table**

![vine_table](https://user-images.githubusercontent.com/104289098/185771969-13be6709-caca-4516-812e-bf4302574ec4.png)


# Deliverable 2

# Amazon_Vine_Analysis

## Our results try to  address the following questions:

- How many Vine reviews and non-Vine reviews were there?
 
**Vine reviews: 90**

![image](https://user-images.githubusercontent.com/104289098/185772220-b4f870a6-8b3a-4729-9135-97487c8c6499.png)

**non-Vine reviews: 37831**

![image](https://user-images.githubusercontent.com/104289098/185772237-f85705f5-ffe9-44fe-807e-cf2d74d6987d.png)


- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
 
**5 Star Vine reviews: 44**

![image](https://user-images.githubusercontent.com/104289098/185772258-785fcd76-c5bb-465d-911f-d1365a41aa8d.png)


**5 Star non-Vine reviews: 14704**

![image](https://user-images.githubusercontent.com/104289098/185772270-1fbe3f8c-735f-4710-8529-0a5fbe9a3a0e.png)


- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
 
**Percentage of 5 stars Vine reviews: 49%**

![image](https://user-images.githubusercontent.com/104289098/185772284-d24cd413-6175-4507-89f4-042fc5d490c0.png)


**Percentage of 5 stars non Vine reviews: 39**

![image](https://user-images.githubusercontent.com/104289098/185772296-b1bd5282-521c-4d2b-b252-90fb8744b280.png)


## Summary: 

The number of 5 star reviews in the Vine program are 49% of the total Vine reviews compared to only 39% in the non-Vine reviews. There is 10% more 5 star reviews in the Vine program which may suggest there is positivity bias in the program. But if we look at the total number of reviews in the Vine program we will see that they only comprise .23% of all reviews which doesn't look that significant or representative of the total reviews. We would need to perform a statistical analysis to get samples and compare each other, or to compare the results in the Vine program to the population and establish if there is a statistical significant difference and be able to better respond if there is a positivity bias in the program. We could  also get the total  5 stars reviews percentage out of the total reviews and see how that number compares with the Vine 5 stars reviews percentage. 

**percentage of paid Vine reviews of the total number of reviews: .23%**

![image](https://user-images.githubusercontent.com/104289098/185773225-94a322f2-0756-4dd7-bba7-3bb053e2efd8.png)


