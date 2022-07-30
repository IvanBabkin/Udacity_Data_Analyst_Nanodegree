# Project 4 - Wrangle & Analyze Data

The aim of this project is to wrangle WeRateDogs Twitter data to create interesting and trustworthy analyses and visualisations. More specifically, the purpose is to use Python and its libraries to gather data from a variety of sources and in a variety of formats. Then, to assess data quality and tidiness before cleaning to prepare it for analysis and finally, to analyse the clean data through visualisations.

## Dataset

The main dataset is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. More specifically, three main pieces of data were collected. 
1. 'WeRateDogs Twitter archive' -> CSV file containing basic tweet data for 2356 WeRateDogs’s tweets.
2. 'Tweet image predictions' -> TSV file containing predicted breed of dog according to a neural network.
3. 'Twitter API file' -> TXT file containing retweet count and favourite count for WeRateDogs’s tweets.

## Summary of Findings

The analysis of data focused on 3 main areas described below:

1. Investigating WeRateDogs' Twitter popularity over time through retweet and favourite counts. The main insights are as follows:
	* The number of favourites has almost always remained higher than the number of retweets over the late 2015 to late 2017 period.
	* Between 2015-11 and 2016-05, the number of favourites was rarely above 5,000. However, after that, the number of favourites exploded, with tweets often getting more than 10,000 favourites.
	* A similar pattern could be observed for the retweet count where between late 2015 and late 2016, the number of retweets rarely passes the 2,500 mark. Meanwhile, in the year 2017, it significantly increases, often reaching 5,000 or more retweets.
	* The number of retweets is closely correlated with the number of favourites with a correlation coefficient 0.91.
2. Investigating the relationship between the 'dog stage' assigned by WeRateDogs and the rating given to the dog. The main insights are as follows:
	* Most tweets did not assign a dog stage. However, when the dog stage was assigned, the most popular dog stage was 'pupper'.
	* The average rating for all 4 dog stages is relatively the same and is around 1.2 (12/10).
	* The regression model showed that there is no statistically significant relationship between dog stage and dog rating.
3. Investigating the relationship between dog breed (predicted from twitter images by neural network) and the number of retweets and favourites. The main insights are as follows:
	* Most tweets did not have a predictable dog breed. However, when the dog breed was predicted, the most popular dog breed was 'labrador retriever'.
	* Pembroke is the dog breed with the highest median favourite count (8696) and median retweet count (2828.5).
	* West highland white terrier dog breed had the lowest median favourite count (2730) and median retweet count (917). 
	* The regression model for retweet count variable found that only three breeds out of the top 10 most popular breeds have statistically significant relationship. These breeds are labrador retriever, pembroke and samoyed.
	* A second regression model for favourite count variable found that the same breeds and staffordshire bullterrier have statistically significant relationship.
