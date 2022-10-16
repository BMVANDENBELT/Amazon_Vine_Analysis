# Amazon_Vine_Analysis
----------------------

# OVERVIEW
----------------------
- The purpose of this project is to analyze Amazon reviews written by members of the paid Vine program by ETL in a pipeline set up for this. I chose to do reviews for Video-Games as I have an appreciation for them. After obtaining the data set, I stored it in an Amazon S3 bucket which I then used Python PySpark to extract/transform the data. Following that, we had to connect the dataframes to an AWS RDS instance and load the extracted/transformed data into a pgAdmin SQL database. To finish the analysis I used PySpark to analyze the data, determining whether or not bias existed towards favorable reviews from Vine members

----------------------

# RESULTS
----------------------
<img width="524" alt="Screen Shot 2022-10-16 at 3 27 59 PM" src="https://user-images.githubusercontent.com/107223178/196054219-0bbc1f99-dca5-4f91-a90d-06f4219c97c2.png">
- Above you will find that 90 reviews were paid for while almost 38,000 were non-paid reviews
<img width="617" alt="Screen Shot 2022-10-16 at 3 30 54 PM" src="https://user-images.githubusercontent.com/107223178/196054334-7f5abeb9-5bc6-40b7-b396-689fcee57baa.png">
- Following that we see that there were almost 44 five-star paid-Vine reviews and almost 15,000 five-star (non-Vine) reviews
<img width="613" alt="Screen Shot 2022-10-16 at 3 33 48 PM" src="https://user-images.githubusercontent.com/107223178/196054449-a49ce9bf-2209-4d41-b921-c3f30f7f3395.png">
- Lastly, it can be shown that there was 48% of Vine reviews that were rated five-star and 38% of non-Vine reviews were rated five-star

----------------------

# SUMMARY
----------------------
- The paid Vine member reviews had almost a 10% higher five-star review which potentially means that there was biased involved in the ratings
- We could also inquire on would be to group each "star-rated" review by a count and put it on a visualization (graph, dashboard, etc.) to see if it displays a correlation in bias and product review
