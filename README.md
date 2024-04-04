## Project Title: Reddit and Yahoo Finance Data Analysis

## Overview
This project retrieves data from Yahoo Finance and Reddit, performs analysis, and visualizes the relationship between Reddit upvotes and comments. It also fetches historical stock data for a specific symbol from Yahoo Finance and conducts a linear regression analysis.

This project involves the analysis of data from the WallStreetBets subreddit on Reddit and financial data from Yahoo Finance, focusing on Tesla, Inc. The goal is to explore potential correlations between Reddit post engagement (upvotes and comments) and stock market performance.

## Data Source

* Reddit_data_pull.ipynb: Jupyter Notebook containing the Python code for data collection, analysis, and visualization.
* README.md: Documentation providing an overview of the project, instructions, and insights.

## Create a config.py file and set the following variables:
* reddit_client_id = "YOUR_REDDIT_CLIENT_ID"
* reddit_secret_key = "YOUR_REDDIT_SECRET_KEY"
* reddit_user_name = "YOUR_REDDIT_USERNAME"
* reddit_password = "YOUR_REDDIT_PASSWORD"
* yahoo_api_key = "YOUR_YAHOO_API_KEY"

## Data Collection

* Reddit Data
Used the Reddit API and the PRAW library to collect information from the "wallstreetbets" subreddit.
Extracted details such as post title, upvotes, comments, and date.
* Yahoo Finance Data
Utilized the Yahoo Finance API to gather real-time and historical data for Tesla, Inc.
Retrieved information like stock symbol, market price, day range, and historical stock prices.

## Obtain API keys:
Reddit: Create a Reddit app [here](https://www.reddit.com/prefs/apps) to get your client ID and secret.
Yahoo Finance: Get your API key from the [RapidAPI Yahoo Finance API](https://rapidapi.com/apidojo/api/yahoo-finance1).

## Dependencies
* Python 3.x
    * Libraries:
    * json
    * requests
    * praw (Python Reddit API Wrapper)
    * pandas
    * matplotlib
    * numpy
    * scipy
      

## Setup
* 		Install the required dependencies using:
bash

Copy codepip install json requests praw pandas matplotlib numpy scipy
* 		Replace the placeholder values in the code with your actual API keys, client ID, secret key, Reddit username, and password.
* 		Run the Python script (Reddit_data_pull2.ipynb) in your preferred environment.

## Usage
* Run the script.
* Enter the stock symbol when prompted.
* Additional search terms can be added for Reddit searches. Press Enter when done.


## Data Analysis
The correlation between subreddit WallStreetBets and stock trends were uncorrelated. 
Upon testing various stock values such as Open price, Close price, and Daily Price Change, with both reddit upvotes and comments, the only significant correlation was between upvotes and comments.


## Reddit Data
* Conducted a linear regression analysis on Daily Change vs. comments to explore their relationship.
![Screenshot 2023-12-12 121933](https://github.com/kaurn6538/Matplotlib_challenge/assets/98873779/52019cfe-1201-48a1-9a0e-372ad6fef1df)
* Ran Spearman’s Rank Correlation Test to determine dependency.


## Yahoo Finance Data
Extracted key financial indicators for Tesla, Inc., such as market price, 52-week range, and average analyst rating.
Obtained historical stock price data for the past 100 days.

# Correlation Analysis

## Merged Reddit and Yahoo Finance data for combined analysis.
Explored potential correlations between Reddit engagement metrics (upvotes and comments) and stock performance.

## Visualization

Created visualizations using Matplotlib to display relationships between Reddit engagement metrics and stock performance.
Plotted linear regression lines to highlight trends.

## Conclusion

* Reddit Engagement vs. Stock Performance: Analyzed the relationship between Reddit post engagement and Tesla stock performance. The linear regression analysis suggests a positive correlation between upvotes and comments, indicating higher engagement for certain stock-related posts.
* Historical Stock Performance: Explored historical stock prices for Tesla, Inc. over the past 100 days. Visualized trends and patterns in the stock's performance.
![Picture1](https://github.com/AprilHolmes7825/Project_1/assets/98873779/8671985b-378b-4b30-97e8-642ba0465f7e)
* Price change and frequency of mentions seem to have only a slight correlation, however the topography of price changes and social media mentions are similar
 Using live data which tracks mentions rather than sentiment, the statistical correlation between the two datasets will be constantly changing. However, we can still use this visualization to track social media’s impact on historical price movement as well as the inverse (price movement affecting frequency of mentions) and use this information to find sleeper stocks, identify targeted price manipulation, and predict trades within the market and amongst members of WallStreetBets


## Suggestions for Further Analysis

* Sentiment Analysis: Incorporate sentiment analysis on Reddit comments to understand the overall sentiment of the community towards specific stocks.
* Volume Analysis: Explore the correlation between stock trading volume and Reddit engagement to identify potential trends or anomalies.

## Instructions for Running the Code

Ensure all dependencies are installed (pip install praw pandas matplotlib requests).
Run the Jupyter Notebook (reddit_yahoo_analysis.ipynb) to execute the code cells sequentially.

## Result
The script outputs visualizations depicting the relationship between Reddit upvotes and comments, as well as historical stock data for the specified symbol.

## Group Members
1.Lee,Ian
2.Christopher Avallon
3.April Holmes
4.Dave Burgman
5.Navdeep Kaur
## Acknowledgments
* Data sourced from Yahoo Finance and Reddit.
* Special thanks to the developers of the used libraries and APIs.

