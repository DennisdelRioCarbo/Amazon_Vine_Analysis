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

The report should contain the following:

## Overview of the analysis: 
The purpose of this project is to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
We accessed a dataset from the Amazon Review Datasets that contains reviews of video games and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Then, we used PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset. The following is  the analysis for the SellBy stakeholders.

## Our results try to  address the following questions:

- How many Vine reviews and non-Vine reviews were there?
**Vine reviews**

![image](https://user-images.githubusercontent.com/104289098/185772220-b4f870a6-8b3a-4729-9135-97487c8c6499.png)

**non-Vine reviews**

![image](https://user-images.githubusercontent.com/104289098/185772237-f85705f5-ffe9-44fe-807e-cf2d74d6987d.png)


- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
**5 Star Vine reviews**

![image](https://user-images.githubusercontent.com/104289098/185772258-785fcd76-c5bb-465d-911f-d1365a41aa8d.png)


**5 Star non-Vine reviews**

![image](https://user-images.githubusercontent.com/104289098/185772270-1fbe3f8c-735f-4710-8529-0a5fbe9a3a0e.png)


- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
**Percentage of 5 stars Vine reviews**

![image](https://user-images.githubusercontent.com/104289098/185772284-d24cd413-6175-4507-89f4-042fc5d490c0.png)


**Percentage of 5 stars non Vine reviews**

![image](https://user-images.githubusercontent.com/104289098/185772296-b1bd5282-521c-4d2b-b252-90fb8744b280.png)


## Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.



