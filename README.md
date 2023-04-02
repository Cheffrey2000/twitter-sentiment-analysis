# Twitter Sentiment analysis
This notebook will allow you to get the current sentiment of a topic from tweets on Twitter. 

# Requirements

> In order to use this script, you must have a Twitter developer account which can be done on the Twitter <a href="https://developer.twitter.com/en">Developer Platform</a>

You will need to store your credentials as local environment variables so the script can access them. The variables you will need are:

* Consumer Key
* Consumer Secret
* Bearer Token

## Usage

After running the first 4 cells you simply need to run the function `get_topic_sentiment`

This function takes one argument which is a string representation of the information you wish to learn about.

Twitter imposes a limit on the number of tweets a basic account can retrieve in one day, so there is a count of 100 requests made in the current state of the function `get_tweets`. To modify this number simply replace it with your desired number of requests. Alternatively you can un-comment the line above which will continue to make the request until the response no longer contains a `next_page` value.

The function returns three elements that represent the counts of each of the sentiment values: Positive, Negative, and Neutral.
