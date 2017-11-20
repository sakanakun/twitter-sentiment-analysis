# twitter-sentiment-analysis
Sentiment Analysis is a branch of Natural Language Processing (NLP) that allows us to
determine algorithmically whether a statement or document is “positive” or “negative”.
Sentiment analysis is a technology of increasing importance in the modern society as it allows
individuals and organizations to detect trends in public opinion by analyzing social media
content. Keeping abreast of socio-political developments is especially important during periods
of policy shifts such as election years, when both electoral candidates and companies can benefit
from sentiment analysis by making appropriate changes to their campaigning and business
strategies respectively.
The purpose of this assignment is to compute the sentiment of text information - in our case,
tweets posted during the 2015 Canadian elections - and answer the research question: “What can
public opinion on Twitter tell us about the Canadian political landscape in 2015?” The goal is
to essentially use sentiment analysis on Twitter data to get insight into the 2015 Canadian
elections.
Central to sentiment analysis are techniques first developed in text mining. Some of those
techniques require a large collection of classified text data often divided into two types of data, a
training data set and a testing data set. The training data set is further divided into data used
solely for the purpose of building the model and data used for validating the model. The process
of building a model is iterative, with the model being successively refined until an acceptable
performance is achieved. The model is then used on the testing data in order to calculate its
performance characteristics.
Produce a report in the form of an IPython notebook detailing the analysis you performed
to answer the research question. Your analysis must include the following steps: data
cleaning, exploratory analysis, model preparation, model implementation, and discussion.
This is an open-ended problem: there are countless different ways to approach each part of
the analysis and therefore the motivation for each step is just as important as its
implementation. When writing the report, make sure to explain (for each step) what it is
doing, why it is important, and the pros and cons of that approach.


The classified data set for this assignment is in a file called classified_tweets.txt . This file
contains tweets that have had their sentiments already analyzed and recorded as binary values 0
and 4. A value of 0 is a negative tweet and a value of 4 is a positive tweet. For this assignment,
the unclassified data set to be analyzed is in unclassified_tweets.txt , which contains a list of
unclassified tweets from the Canadian election.
In classified_tweets.txt , each line is a single tweet, which may contain multiple sentences despite
their brevity. The tweets have been collected directly from the web, so they may contain html
tags, hashtags, and user tags. The comma-separated fields of each line are:
0 class the polarity of each tweet (0 = negative emotion, 4 = positive emotion)
1 id the id of the tweet (e.g. 2087)
2 date the date of the tweet (e.g. Sat May 16 23:58:44 UTC 2009)
3 query the query (e.g. lyx). If there is no query, then this value is NO_QUERY.
4 user the user that tweeted (e.g. robotickilldozr)
5 text the text of the tweet (e.g. Lyx is cool)

● Software
○ Python Version 3.X is required for this assignment. Python Version 2.7 is not
allowed.
○ Your code should run on the Data Scientist Workbench (Kernel 3).
○ All libraries and built-ins are allowed but here is a list of the major libraries you
might consider: Numpy, Scipy, Scikit, Matplotlib, Pandas, NLTK.
○ No other tool or software besides Python and its component libraries can be
used to touch the data files. For instance, using Microsoft Excel to clean the data
is not allowed.
● Required data files
○ classified_tweets.txt: classified Twitter data containing a set of tweets which
have been analyzed and scored for their sentiment
○ unclassified_tweets.txt: unclassified Twitter data containing a set of tweets on
the 2015 Canadian election which needs to be analyzed for this assignment
○ The data files cannot be altered by any means. The IPython Notebooks will be run
using local versions of these data files.
● Optional data files
○ corpus.txt: corpus containing a set of words and their associated sentiment values
○ stop_words.txt: file containing an extensive list of stopwords
○ You may use these files if you wish but you are not required to.
