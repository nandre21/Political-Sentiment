# Identifying Political Shifts

This Shiny app analyzes Reddit comments to extract sentiment and profanity scores based on user discussions in specific subreddits. The application leverages the `RedditExtractoR` package for data fetching and performs sentiment analysis using the `sentimentr` package. By aggregating and visualizing this data, the app provides users with a deeper understanding of public sentiment towards political figures and topics.

## Features

* User-friendly interface allowing input for subreddit, political leaders, and countries.
* Fetches recent comments from specified subreddit.
* Performs sentiment analysis and displays average sentiment for specified entities.
* Visualizes sentiment analysis results using interactive plots.
* Word frequency analysis with filtering of common and irrelevant words.
* Displays top positive and negative comments from the fetched data.
* Option to download sentiment analysis results as a CSV file.

## Getting Started

To run the application, you will need to have R and RStudio installed on your machine. You will also need to install the following R packages:

* shiny
* dplyr
* ggplot2
* plotly
* bslib
* shinycssloaders
* tm
* sentimentr
* RedditExtractoR

You can install these packages using the following command in RStudio:

```r
install.packages(c("shiny", "dplyr", "ggplot2", "plotly", "bslib", "shinycssloaders", "tm", "sentimentr", "RedditExtractoR"))
Once you have installed the required packages, you can run the application by opening the app.R file in RStudio and clicking the "Run App" button.

Usage
To use the application, simply enter the subreddit name and names of political leaders or countries for sentiment analysis in the input fields on the left side of the application. Then click the "Fetch Comments" button to fetch the comments from Reddit and perform the sentiment analysis. The results of the sentiment analysis will be displayed on the right side of the application.

Project Significance
The sentiment analysis of Reddit comments regarding political leaders and policies provides invaluable insights into public opinion and can serve as a predictive tool for political forecasting. Understanding how sentiment evolves can indicate shifts in public support, revealing whether a leader is in danger of being ousted or if policies are gaining traction among the populace.

Project Potential
Real-Time Analysis: The project provides real-time insights into public sentiment by analyzing recent Reddit comments.
Predictive Power: Sentiment analysis can be used as a forecasting tool to predict potential political crises or shifts before they manifest in the real world.
Data-Driven Decision Making: Policymakers, political analysts, and campaign strategists can leverage this tool to inform their strategies based on public sentiment towards specific policies or leaders.
Public Engagement: The project democratizes data analysis by providing accessible insights to the public.
Interdisciplinary Approach: The project employs advanced computational techniques to extract insights from social media, highlighting the growing importance of data analytics in political science.
Mathematics Behind Sentiment Analysis
The core of sentiment analysis in this project relies on deriving sentiment scores from text data. Each comment is processed to assign a sentiment score based on the sentiment orientation of individual words. The sentiment score for a comment is computed as the sum of the sentiment scores of individual words, normalized for the number of words in the comment. Sentiment scores can range from -1 (very negative) to +1 (very positive), with scores near 0 indicating neutrality.

Filtering Words
The project also filters out irrelevant and common words to enhance the accuracy of the sentiment analysis. Words filtered include stop words, profane words, and irrelevant words.

Conclusion
This Shiny app serves as an innovative tool for analyzing sentiment and profanity in Reddit comments, providing insights into public opinion on political leaders and countries. By interpreting sentiment scores and understanding trends, users can foresee potential political changes and the public's reaction to political events. This project not only enhances the ability to engage with current political discourse but also empowers researchers, policymakers, and interested citizens to understand the dynamics of public sentiment in an increasingly digital world.

Contributing
Contributions to this project are welcome. If you find a bug or have a suggestion for a new feature, please open an issue on the GitHub repository. If you would like to contribute code, please fork the repository and submit a pull request with your changes.
