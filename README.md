# Reddit-Muncher
This tool was built used for a stock prediction project. It takes a list of reddit posts in csv format that have been previously partitioned by company. It then analyzes the sentiment of the posts computing daily averages.

It utilizes the vader sentiment analyzer from NLTK. Vader works best on small sentences, so posts are first split by sentence, which are then individually analized.

The following features are then computed

1) Mean of the compound score of each sentence in a post
2) The compound score of the most positive sentence
3) The compound score of the most negative sentence
4) The mean negative score of all sentences
5) The mean positive score of all sentences

These scores are then averaged for every post seen that day and the number of posts on that day is also included in the data set.
