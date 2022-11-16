# sentiment_analysis 
This projects builds a model that learns the relationship between textual inputs and their associated sentiment (good or bad) using logistic regression. 

The function process_tweet processes a given tweet by lowercasing, removing stopwords and punctuations, tokenizing and stemming.

All words in the group of string inputs are put in a list of unique words to build a vocabulary.

Two separate corpuses are defined based on sentimental categorization, that is, positive corpus and negative corpus.

For each word in the vocabulary, its frequency in both the positive and negative corpuses (freq_pos, freq_neg) are computed.

The list [1.0, freq_pos, freq_neg] for each tweet, obtained by summing over words in the tweet, is used to train a logistic regression model, using a gradient descent training algorithm.

Model achieved 99.5% accuracy when applied on the test set.
