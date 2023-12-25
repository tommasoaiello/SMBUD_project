# Systems and methods for big and unstructured data 2023/2024



## Overview

This project is part of a course named 'Systems and Methods for Big and Unstructured Data'. The dataset consists in Trump Twitter Archive. The goal of the project is to make 10 queries on the dataset using Elastic Search.
## Dataset

The dataset used for analysis is the "trump_tweets_archive" downloaded from kaggle (https://www.kaggle.com/datasets/headsortails/trump-twitter-archive) containing tweets attributed to the former U.S. President Donald Trump. The dataset was made public by Brendan of https://www.thetrumparchive.com/

The dataset consists of more than 56k Trump's tweets with various attributes such as tweet id, text, is_retweet, is_deleted, device, favorites, retweets, datetime, is_flagged, date. The goal of the project is to perform meaningful queries using ElasticSearch and visualize the results in Kibana.

## Queries

The project involves a series of 10 queries with increasing complexity, exploring different aspects of the dataset. These queries cover a range of topics, from basic filtering and aggregation to more advanced queries involving date ranges, keyword searches, and analysis of flagged tweets.

1. Get all the tweets that contain at least the word 'Biden' or 'Sleepy Joe' and that also include at least one word between 'election', 'fraud', 'rigged', 'vote', 'fake'
2. Get all the tweets that contain atleast one word between 'Biden' and 'Sleepy Joe' and that also include at least one word between 'election', 'fraud', 'rigged', 'vote', 'fake'. 
Count the ones that are flagged which means that X (aka Twitter) decided to flagbecause they were considered harmful or against the policies.
3. Get the average retweets and favorites per tweet containing words that may be related to elections and what happened during the protests after the presidential elections of 2020.
4. Get the monthly tweet count.
5. Get the tweets that contain the word economy or similar using fuzziness. And sort them i ascending order. Not perrfect matches have lower scores
6. Retreive tweet and datetime of the tweet with most retweets per year.
7. Retrieve tweets having at least one word that is covid, virus, vaccine. That are not retweet and that are made in 2020. Get the aggregate count by month and get the one with maximum retweet.
8. Get the average retweet and favorite per tweet per month related to china and virus and vaccine. That is not a retweet and tht was written in 2020.
9. Get the number of tweets per year that were deleted. And for each year get the text and datetime of the one with most favorites.
10. Get the tweet count per month of tweets containing 'Hillary' or 'Clinton' or 'democrats' made in 2016 and get the tweet count per month of tweets containing 'Biden' or 'Sleepy Joe' or 'democrats' in 2020.

## Instructions

1. Ensure ElasticSearch and Kibana are installed and running.
2. Import the "trump_tweets_archive" dataset into ElasticSearch.
3. Execute the provided queries in Kibana's Dev Tools or through the appropriate API calls.
4. Explore the visualizations and results in Kibana to derive insights from the dataset.


