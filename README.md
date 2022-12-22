# Amazon_Vine_Analysis
# Overview
The purpose of this project is to perform data analysis on amazon’s video game reviews. More specifically, I was examining if there were any bias on the reviews based on if they were in  the Vine (paid) program. I, first downloaded the data and stored it into AWS services, namely, S3 buckets. From there, I used PySpark to gather the data from my S3 bucket instance and store it into a table/dataframe and then I ran analysis on the data.

# Results
![Results_Img1](/Resources/VineReviews.PNG)
![Results_Img2](/Resources/FiveStarVineReviews.PNG)
As seen from the image above, the total number of Vine reviews are 4,291 and non-Vine reviews are 1,781,706. Amongst the Vine reviews, there were only 1,607 five star reviews and amongst the non-Vine reviews, there were 1,025,317 five star reviews. Lastly, I calculated that 99.84% of the five star reviews were from non vine users and only 0.16% of the five star reviews came from the vine users.

# Summary
According to the results I achieved, I found out that ~37% of the vine users (out of 4,291) gave five star reviews, however, ~57% of the non vine users (out of 1,781,706) also gave five star reviews. Thus, I cannot see any bias on the five star reviews that came from the vine users. 
Besides checking the percentage of five star vine users and non five star vine users, I can also run an additional analysis among vine users and categorize them by the star rating they gave and calculate the percentage of review for each star rating.
