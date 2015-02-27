# must-read-sentimentAnalysis
List of Resources for Sentiment Analysis in General and including resources for Arabic Language as well.
The list is under continous update.

## Papers:
### Sentiment Classification : 
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

### Sentiment Analysis in Arabic Language:
1. [Abbasi et al. Sentiment Analysis in Multiple Languages: Feature Selection for Opinion Classification in Web Forums](http://128.196.40.18/intranet/papers/AhmedAbbasi_SentimentTOIS.pdf) 
  - very good categorized literature reviews about common features selected, techniques, domains of use in sentiment analysis
  - uses Entropy Weighted Genetic Algorithm to do feature selection among each of the previous techniques
2. [El-Beltagy, Samhaa R., and Ahmed Ali. "Open issues in the sentiment analysis of arabic social media: A case study." Innovations in Information Technology (IIT), 2013 9th International Conference on. IEEE, 2013.](http://tmrg.nileu.edu.eg/resources/publications/Samhaa_OpenIssuesintheSentiment_IIT2013.pdf)
  - overview of main issues and obstacles in arabic social media sentiment analysis 
  - semi-automatic generation of ~4k entries egyptian dialect sentiment lexicon (link available in the paper) using  conjunctions 
  - Evaluation of Generated Lexicon
3. [Abdul-Mageed & Diab. "AWATIF: A Multi-Genre Corpus for Modern Standard Arabic Subjectivity and Sentiment Analysis." LREC. 2012.](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.383.4662&rep=rep1&type=pdf)
  - Main usefulness : Good regulations for annotating sentiment datasets 
  - multi-genre annotated corpus of Modern Standard Arabic for SA
  - built from different resources including Penn Arabic Treebank, Wikipedia Talk Pages and Web forums
  - manually annotated :
    - with Guidlines or simple Guidelines
    - with Trained Annotators/ Crowdsourcing 
    - elaborate the importance of guidelines and training of annotators to produce dependable annota-tions
    - dataset not publicly available

## Books:

1.  [Bing Liu : Sentiment Analysis and Opinion Mining ](http://www.cs.uic.edu/~liub/FBS/SentimentAnalysis-and-OpinionMining.pdf) 
Book is a thorough literature review in various issues of sentiment analysis, this could be nice to get the big picture of sentiment analysis and also to  get related work in any of the issues of sentiment analysis.


## Courses:

1. [NLP - Stanford,  Dan Jurafsky & Christopher Manning] (https://www.coursera.org/course/nlp)


## Datasets:
### English Datasets : 
- Pang & LEE movie reviews:
  - Size : 2K , 1000 positive and 1000 negative
  - [homepage](http://www.cs.cornell.edu/people/pabo/movie-review-data/)
  - [Paper](http://www.cs.cornell.edu/home/llee/papers/sentiment.pdf)
- SNAP - Web data: Amazon reviews
  -  size : 34,686,770 Reviews 
  -  [homepage](http://snap.stanford.edu/data/web-Amazon.html)
  -  [Direct links](http://snap.stanford.edu/data/amazon/)
  -  [Paper](http://i.stanford.edu/~julian/pdfs/recsys13.pdf)

### Arabic Datasets & Lexicons :
- LABR: Large Arabic book database from bookreviews
  - Size : 36K
  - [homepage](http://www.mohamedaly.info/datasets/labr)
  - [Paper](http://www.aclweb.org/anthology/P13-2088)

- Large Arabic Resources for Arabic Sentiment Analysis :
  - Datasets of 33K reviews in Movies, Hotels, Restaurants, Products domain 
  - Generated Lexicon of 2K entries in domains of Books, Movies, Hotels, Restaurants and Products
  - Benchmarking of standard machine learning techniques and feature representation methods over the datasets
  - Available Code for Experiments as a starter kit for baseline classifiers
  - [homepage](https://github.com/hadyelsahar/large-arabic-sentiment-analysis-resouces)
  - Paper : [ElSahar, Hady, and Samhaa R. El-Beltagy. "Building Large Arabic Multi-Domain Resources For Sentiment Analysis." Computational Linguistics and Intelligent Text Processing. Springer Berlin Heidelberg, 2015.](https://www.dropbox.com/s/993lf5jj0oooq4b/Paper%201%20-%20Building%20Large%20Arabic%20Resources%20for%20Sentiment%20Analysis.pdf?dl=0)
  
- Unweighted Opinion Mining Lexicon
  - An Arabic sentiment Lexicon consisting of 4392 entries mostly of Egyptian dialect (file is .csv, unicode). Compound entries (idioms and expressions are unstemmed). Other entries are prefix stemmed but postfix unstemmed.
  - [Download[(http://tmrg.nileu.edu.eg/resources/datasets/unWeightedOMLexicon.csv)
  - Paper : [El-Beltagy, Samhaa R., and Ahmed Ali. "Open issues in the sentiment analysis of arabic social media: A case study." Innovations in Information Technology (IIT), 2013 9th International Conference on. IEEE, 2013.](http://tmrg.nileu.edu.eg/resources/publications/Samhaa_OpenIssuesintheSentiment_IIT2013.pdf)
- Arabic Slang Lexicon for Twitter Sentiment Analysis :
  - Lexicon of ~400 terms build automatically from Matching tweets to lexico-syntactic patterns
  - Paper : [ElSahar, Hady, and Samhaa R. El-Beltagy. "A fully automated approach for arabic slang lexicon extraction from microblogs." Computational Linguistics and Intelligent Text Processing. Springer Berlin Heidelberg, 2014. 79-91.](https://www.dropbox.com/s/xbuavbdgok54er1/Elsahar%20Elbeltagy%20automatic%20lexicon%20extraction%20from%20microblogs%20.pdf?dl=0)
  - [Download](https://github.com/hadyelsahar/must-read-sentimentAnalysis/blob/master/resources/slang-lexicon.csv)


## People : 

## Glossary :
[The Natural Language Processing Dictionary](www.cse.unsw.edu.au/~billw/nlpdict.html) : Glossary contains definitions of wide range of used terms in Natural language processing topics, very useful when reading papers.

## Miscellaneous:
1. [Chris. Manning : deep learning without magic part 1](http://techtalks.tv/talks/deep-learning-for-nlp-without-magic-part-1/58414/) : 
  main interesting points : 
  - Representing each word by a feature vectors built from words in context
  - Using Deep Neural networks to adapt those feature weights 
  - use those adapted feature vectors in multiple NLP classification problems
  - the old way : [AL Maas et al. : Learning Word Vectors for Sentiment Analysis](http://ai.stanford.edu/~ang/papers/acl11-WordVectorsSentimentAnalysis.pdf)


-----
### Contributing:
Feel Free to Send a [pull Request](https://help.github.com/articles/using-pull-requests/) with any updates you think it's good to add 
