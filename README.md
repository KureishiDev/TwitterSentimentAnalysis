# Twitter Sentiment Analysis

This repository contains a Python script for collecting, processing, and analyzing tweets to perform sentiment analysis. The script uses the Tweepy library to collect tweets from Twitter based on a keyword or hashtag, and it uses the VADER sentiment analysis tool to classify the sentiment of each tweet as positive, negative, or neutral. Additionally, it performs exploratory data analysis (EDA) and visualizes various aspects of the data.

## Project Structure

The script performs the following tasks:

### 1. Twitter API Configuration and Data Collection
- Configures the Twitter API using `Tweepy` and collects tweets containing a specified keyword or hashtag (in this case, "Python").
- Retrieves 100 tweets and stores them in a DataFrame with information like tweet ID, text, creation date, retweet count, and like count.

### 2. Data Preprocessing and Cleaning
- Cleans the tweet text by removing URLs, mentions, hashtags, and non-alphanumeric characters.
- Converts the text to lowercase for consistency.

### 3. Sentiment Analysis
- Uses the `VADER` sentiment analysis tool to classify each tweet's sentiment as 'Positive', 'Negative', or 'Neutral'.
- Adds the sentiment classification to the DataFrame.

### 4. Exploratory Data Analysis (EDA)
- Visualizes the distribution of tweet sentiments using a bar chart.
- Displays the most common words for each sentiment (positive, negative, neutral).
- Plots the relationship between sentiment and retweet count using a boxplot.
- Plots the relationship between sentiment and like count using a boxplot.

## Requirements

To run this script, you will need the following Python libraries:
- `tweepy`
- `pandas`
- `nltk`
- `matplotlib`
- `seaborn`
- `re`

You can install them using pip:

pip install tweepy pandas nltk matplotlib seaborn

## Usage

1. Set up your Twitter Developer account and obtain your API keys. Replace the placeholders in the script (`SUA_CONSUMER_KEY`, `SUA_CONSUMER_SECRET`, `SEU_ACCESS_TOKEN`, `SEU_ACCESS_TOKEN_SECRET`) with your actual credentials.
2. Run the script to collect tweets and perform sentiment analysis.

python twitter_sentiment_analysis.py

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
