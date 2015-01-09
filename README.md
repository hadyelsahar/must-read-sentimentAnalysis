# must-read-sentimentAnalysis
List of Resources for Sentiment Analysis Researcher Starter


### Papers:

1.  [Turney 2002 : Thumbs up or thumbs down?](http://dl.acm.org/citation.cfm?id=1073153)
  - everyone starts withthis paper, probably because it’s the oldest notable work there in sentiment classification,
  turney using two words “excellent” and “poor” and point wise mutual PMI information to do unsupervised sentiment classification 
2. [Pang, Lee 2002 : Thumbs up?: sentiment classification using machine learning techniques](http://dl.acm.org/citation.cfm?id=1118704)
cited 3K times also for the same reason above, paper in bullets : 
  - Published a movie reviews dataset that everyone uses until now 
  - used Machine learning classifiers for  3 k-folds crossvalidation
  - features were basic bag of words (unigrams and/or bigrams) word existence, word freq ( no tfidf )
  - other additional features : top unigrams, adjectives, position
  - compared results to results of features manually selected by two manual annotators 
  - Accuracy of baseline (manual annotated features ~60-70%) 
  - Accuracy of ML ~80-83%

### Books:

1.  [Bing Liu : Sentiment Analysis and Opinion Mining ](http://www.cs.uic.edu/~liub/FBS/SentimentAnalysis-and-OpinionMining.pdf) 
Book is a thorough literature review in various issues of sentiment analysis, this could be nice to get the big picture of sentiment analysis and also to  get related work in any of the issues of sentiment analysis.


### Courses:

1. [NLP - Stanford] (https://www.coursera.org/course/nlp)


### Datasets:


### Miscellaneous:
1. [Chris. Manning : deep learning without magic part 1](http://techtalks.tv/talks/deep-learning-for-nlp-without-magic-part-1/58414/) : 
  main interesting points : 
  - Representing each word by a feature vectors built from words in context
  - Using Deep Neural networks to adapt those feature weights 
  - use those adapted feature vectors in multiple NLP classification problems
  - the old way : [AL Maas et al. : Learning Word Vectors for Sentiment Analysis](http://delivery.acm.org/10.1145/2010000/2002491/p142-maas.pdf?ip=41.47.2.56&id=2002491&acc=OPEN&key=4D4702B0C3E38B35.4D4702B0C3E38B35.4D4702B0C3E38B35.6D218144511F3437&CFID=616814785&CFTOKEN=59548436&__acm__=1420792051_5954d0255276523b3ae24e158ee51d1a)


-----
### Contributing:
Feel Free to Send a [pull Request](https://help.github.com/articles/using-pull-requests/) with any updates you think it's good to add 
