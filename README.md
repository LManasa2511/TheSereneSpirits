Finance News Aggregator
Table of Contents
Overview
Setup
Usage
Support These Projects
Overview
Current Version: 0.1.2

Investors use news articles to gain an idea of market sentiment and hopefully be able to predict the direction of markets based on the sentiment of these articles and how they are published. The finnews library is designed to help the collection of news articles related to business topics and market news easy and efficient.

Setup
To install the library, run the following command from the terminal.

pip install fin-news
To upgrade the library, run the following command from the terminal.

pip install --upgrade fin-news
Usage
Here is a simple example of using the finnews library to to grab the top stories on CNBC.

from pprint import pprint
from finnews.client import News

# Create a new instance of the News Client.
news_client = News()

# Grab the CNBC News Client.
cnbc_news_client = news_client.cnbc

# Grab the top news.
cbnc_top_news = cnbc_news_client.news_feed(topic='top_news')

# Print it.
pprint(cbnc_top_news)
