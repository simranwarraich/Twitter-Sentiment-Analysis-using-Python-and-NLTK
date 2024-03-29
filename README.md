# Twitter-Sentiment-Analysis-using-Python-and-NLTK

Sentiment analysis, a powerful branch of NLP, aims to automatically understand the emotional tone (positive, negative, or neutral) within a piece of text. It's like having a computer program that can gauge public opinion by analyzing the emotions expressed in written content.
<p><img src = "79592twitter.jpg"></p>
In this project, sentiment analysis is used to analyze tweets about the movie "Avengers: Endgame." By deciphering the sentiment (polarity) and the level of opinion (subjectivity) within these tweets, we can gain valuable insights into public perception of the movie and its cast members.

**Polarity:** This refers to the positive, negative, or neutral sentiment expressed in a text. A positive polarity score indicates a favorable opinion, while a negative score suggests an unfavorable one.

**Subjectivity:** This measures the extent to which a text expresses an opinion or personal view. A high subjectivity score indicates a strong opinion, while a low score suggests a more factual statement.

# Project Goal:
1. Analyze sentiment of tweets related to "Avengers: Endgame"
2. Understand public perception of the movie and its cast members

# Project Structure:
The project consists of the following files:
1. README.md: This file (you are reading it now!) provides an overview of the project.
2. [twitter-sentiment-analysis-using-python-and-nltk.ipynb](twitter-sentiment-analysis-using-python-and-nltk.ipynb):Contains the main script for exploreing public sentiment towards the movie "Avengers: Endgame" using Python libraries for NLP (Natural Language Processing). It leverages the Twitter API to collect tweets and performs sentiment analysis with NLTK and TextBlob..
   
# Steps:
The code performs sentiment analysis on tweets related to the movie "Avengers: Endgame" using the Twitter API, NLTK, and TextBlob libraries. Here's a breakdown of the main steps:

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

# Who,When,Why?
**Author:** Simran Warraich
**Version:** 1


