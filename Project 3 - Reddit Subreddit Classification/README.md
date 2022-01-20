# GA DSI 26: Project 3 - Reddit Subreddit Classification
***

## Problem Statement
***
As an employee at a computer building company in Singapore, the company receive many requests from customers regarding new computer build and after sales support for their PC. The volume of requests has increased and is requiring more staff to sort and classify these requests between PC building queries or after-sales support for their computer. Hence, the company wants to build a classification model to sort and classify future incoming requests into the two categories of PC building queries or after-sales support.

As the company does not archive and store past queries sent to the company, to build this classification model, the Reddit posts in two relevant subreddits shall be used in place of real customers questions to train and test the model. The subreddits identified are `r/buildapc` and `r/techsupport`. 

## Executive Summary
***
|            Results from the models            | Train Score | Test Score | Best Score |
|:---------------------------------------------:|:-----------:|:----------:|------------|
| Baseline Accuracy                             |    0.512    |    0.510   |     --     |
| CountVectorizer with Multinomial Naive Bayes  |    0.883    |    0.859   |    0.837   |
| TfidfVectorizer with Multinomial Naive Bayes  |    0.877    |    0.869   |    0.845   |
| CountVectorizer with Random Forest            |    0.872    |    0.838   |    0.827   |
| TfidfVectorizer with Random Forest            |    0.883    |    0.832   |    0.822   |
| CountVectorizer with Logistic Regression      |    0.962    |    0.827   |    0.815   |
| TfidfVectorizer with Logsitic Regression      |    0.926    |    0.861   |    0.834   |

After testing 6 models, the best performing model to classify incoming queries into the two categories of queries relating to building a PC or after sales support for the computer purchased from the company would be the TfidfVectorizer with Multinomial Naive Bayes. The model is able to correctly classify 86.9% of the posts. There would still be room for improvement to cater for the remaining 13.1% of posts that would be wrongly classified.

With this model, the company can implement this model as automated first step of classification for incoming queries without need for human oversight as it is able to correctly classify the incoming queries at a high success rate. Subsequently, as the staff reviews the queries and finds out it is wrong, they can transfer the queries across to the correct department while flagging the wrong query for further analysis to improve the model.

## Data Dictionary
***
The following is the data dictionary for the datasets used in this project.

|   Feature   | Type |            Dataset            |                                         Description                                        |
|:-----------:|:----:|:-----------------------------:|:------------------------------------------------------------------------------------------:|
|  subreddit  |  int |             merged            | Subreddit which the posts belong to and 0 refer to r/buildapc and 1 refer to r/techsupport |
|  subreddit  |  str |     buildapc, techsupport     |                             Subreddit which the posts belong to                            |
| text_tokens |  str | merged, buildapc, techsupport |       Tokenized and lemmatized words combined from combined text of both subreddits.       |
|    title    |  str |     buildapc, techsupport     |                                 Title of post in subreddit                                 |
|   selftext  |  str |     buildapc, techsupport     |                             Text in the main post in subreddit                             |
|     text    |  str |     buildapc, techsupport     |                     Combined text from title and selftext of subreddits                    |
|   text_len  |  int |     buildapc, techsupport     |                              Length of posts from text column                              |


