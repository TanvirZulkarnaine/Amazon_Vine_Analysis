# Amazon_Vine_Analysis
# Overview
The purpose of this project is to perform data analysis on amazon’s video game reviews written by members of the paid Amazon Vine Program. Companies like to play a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. I was examining to see if there were any bias on the reviews based on if they were in  the Vine (paid) program. 
I have performed ETL process on the Amazon’s video game review dataset. I, first downloaded the data and stored it into AWS services, namely, S3 buckets. After that, I used PySpark to gather the data from my S3 bucket instance and store it into a table/dataframe and then I ran analysis on the data. Then I connected AWS RDS instance to load my transformed data into pgAdmin. Lastly, I used PySpark, and SQL queries to determine if there were any bias towards favorable reviews from Vine members in the dataset.

# Results
![Results_Img1](/Resources/VineReviews.PNG)
![Results_Img2](/Resources/FiveStarVineReviews.PNG)
As seen from the image above, the total number of Vine reviews are 4,291 and non-Vine reviews are 1,781,706. Amongst the Vine reviews, there were only 1,607 five star reviews and amongst the non-Vine reviews, there were 1,025,317 five star reviews. Lastly, I calculated that 99.84% of the five star reviews were from non vine users and only 0.16% of the five star reviews came from the vine users.

# Summary
According to the results I achieved, I found out that ~37% of the vine users (out of 4,291) gave five star reviews, however, ~57% of the non vine users (out of 1,781,706) also gave five star reviews, which is a higher percentage and also contains higher number reviewers than vine user reviews. Thus, I do not believe there are any bias on the five star reviews that came from the vine users. 
Besides checking the percentage of five star vine users and non five star vine users, I can also run an additional analysis among vine users and categorize them by the star rating they gave and calculate the percentage of review for each star rating.
