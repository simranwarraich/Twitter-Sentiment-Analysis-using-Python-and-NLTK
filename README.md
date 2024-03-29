# Twitter-Sentiment-Analysis-using-Python-and-NLTK

This code performs sentiment analysis on tweets related to the movie "Avengers: Endgame" using the Twitter API, NLTK, and TextBlob libraries. Here's a breakdown of the main steps:

1. **Authenticate to Twitter API**: The code authenticates to the Twitter API using the provided API keys and tokens.

2. **Get Tweets**: It retrieves up to 15,000 tweets containing the hashtag #AvengersEndgame and stores them in a list which is then converted to a pandas DataFrame.

3. **Preprocess Tweets**: The tweets are preprocessed by removing URLs, mentions, stopwords, punctuation, and converting to lowercase. Additionally, it identifies if a tweet mentions a specific cast member (e.g., Iron Man, Captain America, Thor) and creates a corresponding flag column.

4. **Calculate Sentiment**: The polarity (sentiment score) and subjectivity scores are calculated for each processed tweet using TextBlob.

5. **Analyze Cast Member Sentiment**: Sentiment data (mean polarity and subjectivity) is calculated for each cast member.

6. **Visualize Sentiment**: Several visualizations are generated:
   - Bar charts for mean polarity and subjectivity by cast member
   - Line plots for moving average polarity over time for each cast member
   - Line plot for moving average polarity over time for all tweets
   - Word clouds for each cast member based on their mentioned tweets

The code includes detailed comments explaining each step and the functionality of the helper functions used throughout the analysis.

To use this code, you'll need to provide your Twitter API credentials (consumer key, consumer secret, access token, and access token secret) and ensure that you have the required libraries installed (tweepy, pandas, matplotlib, nltk, textblob, and wordcloud).
