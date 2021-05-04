# iPhone 12 Tweet Sentiment Analysis Using Tweepy API in Python


# Introduction

- iPhone 12 tweet analysis aims at analyzing tweets that users have made in response to the newly launched iPhone 12 by Apple company. The goal is to study what the users think about the product. Twitter, being a platform to opinions and experiences of users, and to communicate directly with concerned people, was chosen as a good source to extract information about iPhone 12.


# Contents

- [The Data Set](#the-data-set)
  - [Data Selection](#data-selection)
  - [Data Wrangling](#data-wrangling)
  - [Exclusion Criteria](#exclusion-criteria)
- [Used Tools](#used-tools)
- [Conclusion](#conclusion)
- [Follow Me On](#follow-me-on)

# The Data Set

### Data Selection
- Tweets related to iPhone 12 were scraped from Twitter using an open-source python package known as Tweepy API. Attributes extracted from the tweets are 
  - tweet_id: Unique number for each user
  - Username: Username of the user
  - User_description: Description of user
  - User_followers: Number of followers per user
  - User_following: Number of followings per user
  - User_location: Location of user
  - Date_Time: Date & time of the tweet
  - tweet: Text of the tweet 
  - Hashtags: Hashtags extracted from the tweets
  - Likes: Number of likes on the tweet
  - Retweet_count: Number of retweets for the tweet
  - source: Device from which the tweet was posted
  - tweet_place: Location of the tweet when posted
  - tweet_is_quote_status: Retweet with a comment
  - tweet_language: Language of the tweet
  - tweet_coordinates: Location coordinates of tweet

### Data Wrangling
- Hashtags were pre-processed in order to remove the attached index numbers while scrapping the tweets.
- Pre-processing of tweets was conducted in various steps as mentioned below:
  - Transformation of tweet to lower case.
  - URL’s, numbers and special characters were excluded.
  - Expansion of English language contractions.
  - Finally, tokenizing the tweets and applying lemmatization technique on it.

### Exclusion Criteria

- Due to readability constraint, tweets which were only in English language were considered. Moving further, tweets were considered before the product was launched for users and due to the limitations of open source Tweepy API we were able to scrape tweets within a range of 7 days only. Session time-out error occurred if we tried to scrape large number of tweets, so we had to scrape multiple times with a smaller number in order to obtain large number of tweets.

# Used Tools
 - Jupyter Notebook
 - Model Creation
   - Latent Dirichlet Allocation (LDA)
   - Non Negative Matrix Factorisation (NMF)
   - Aspect Based Sentiment Analysis (ABSA)

# Conclusion
- It was observed post analysis that majority of the tweets extracted were either positive or neutral. In explanation to this, tweets were scrapped before the product was launched publicly. So, it might be that people were positive about the new product and expecting that the product will be good.
- We believe that most of the tweets are positive and neutral, and this might change once the users get a hands-on experience and be able to relate to the new features and its practical use. If it doesn’t meet the expectations of the user, they might tweet.

# Follow Me On
http://linkedin.com/in/shreshthrathod
