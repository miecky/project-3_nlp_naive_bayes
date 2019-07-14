# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Web APIs & Classification

### Executive Summary

Four open problmes in Natural Language Processing (NLP) were discuessed at Deep Learning Indaba 2018, which are **natural language understanding**, **NLP for low-resource scenarios**, **reasoning about large or multiple documents**, and **datasets, problems, and evaluation**. Understanding the performance, limitation, and possible improvement of the learning algorithms is the fundation for building more capable ones to solve more challenging problems. This project focuses on the performance of the **multinomial naive Bayes (MNB)** algorithm through comparing it against **logistic regression** on the classification of posts from two subreddits (i.e., r/breastcancer and r/airpollution) of Reddit.com. I also took one step further to replicate the MNB modeling results to understand the mechanism behind this frequently used text classifier.  

Total 1887 posts (i.e., 904 from r/airquality and 983 from r/breastcancer) were obtained through Reddit.com's web API using Python. Through Train/Test split, the models were trained with the title of 70% of the training data (i.e., 1315 posts). The goal was to classified the 30% test data (i.e., 572 posts) based on their titles using the trained model. The titles were split in to words (including numerical values) using tokenizer, and grouped into simple vocabulary form using lemmatization. A bag-of-word approach was used through CountVectorizer and TFIDFVectorizer transformation. For the logistic regression model, LASSO regulization was used. A series of hyperparameters including minimum and maximum numbers of features, ngram range, and whether or not removing stop words were iterated through **Pipeline** and **GridSearchCV**. 

The results shows that the logistic regression with CountVectorizer classified test posts with 100% accuracy, which is the best of the four models. Due to the great difference of the two subreddits, all four models produces near perfect accuracy with both train and testing data. The difference between MNB and Logistic Regression is trivial. The two posts misclassified by MNB could be easily classified by human. The MNB classifier results for selected documents were reproduced and presented in Part 2 of the presentation.

Overall, MNB and logistic regression both produces near perfect results due to the great difference of the two posts. For documents with distinguishable topics, feature improve mechanism such as TFIDFVectorizer shows little or no improvement to the models. To further understand the limitation and investigate the improvement potential of the MNB model, the following further steps are considered:

1. Test on multiclass documents with more similar topics.
2. Investigate the scenario when MNB fails.
3. Try "transformed weight-normalized complement naive Bayes" (TWCNB) discussed in paper published by University of Waikato, Hamilton, Newzealand.


