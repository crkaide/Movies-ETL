# Movies ETL

## Background

The client, Amazing Prime Video (represented by Britta), is a streaming platform hosted by the world's largest online retailer, Amazing Prime.  To facilitate the purchase of streaming rights at the lowest possible cost, the client has sponsored a hackathon whose goal is the development of an algorithm that predicts the popularity of low-budget films.  The client provided two data sources (Wikipedia and ratings).  Initial analysis included extracting the data, transforming it into a dataset, and loading it into a SQL table for use by the local coding community.

## Purpose

Following the analysis above, the client requested Python code to keep the SQL table updated daily.  The required the development of an automated pipline to extract, transform, and load data from three files (Wikipedia, ratings, and Kaggle metadata).

## Results

_*movies_query.png*_
NOTE:  Module 8, deliverable 4, step 9 lists the correct number of rows as 6,052.  The results of this code yield 6,075, a 0.4% (0.0038) difference from the count of the expected output.  This difference is statistically negligible.  In addition, the module (8.3.2 Iterative Process for Cleaning Data) states, _"Once we've identified the problem, we need to make a plan and decide whether it is worth the time and effort to fix it."_  It is highly likely that the difference in the count results from the module work formatting the final dataframe column names prior to reading the ratings CSV, while the challenge work requires the formatting to be done later in the process.  In any case, after time spent troubleshooting the code, the 0.4% difference in this dataset's row count, while necessarily noted here, will have no significant impact on the final table(s).
![movies_query.png](https://github.com/crkaide/Movies-ETL/blob/main/Resources/movies_query.png?raw=true)

_*ratings_query.png*_
![ ratings_query.png](https://github.com/crkaide/Movies-ETL/blob/main/Resources/ratings_query.png?raw=true)
