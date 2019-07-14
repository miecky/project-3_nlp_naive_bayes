# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Web APIs & Classification

### Description

This project covers three of the biggest concepts: Classification Modeling, Natural Language Processing and Data Wrangling/Acquisition.

Part 1 of the project focuses on **Data wrangling/gathering/acquisition**. This is a very important skill as not all the data will be in clean CSVs or a single table in SQL.  There is a good chance that one will have to gather some data from some unstructured/semi-structured sources; when possible, requesting information from an API, but often scraping it because they don't have an API (or it's terribly documented).

Part 2 of the project focuses on **Natural Language Processing** and converting standard text data (like Titles and Comments) into a format that allows us to analyze it and use it in modeling.

Part 3 of the project focuses on **Classification Modeling**.  Compare various models, means of assessment and preprocessing associated with classification.

### Goal
1. Using Reddit's API to collect posts from two subreddits.
2. Use NLP to train a classifier on which subreddit a given post came from. This is a binary classification problem.
3. Take a closer look at the Naive Bayes Model and understand how model classifies the posts.


### Directory Structure
```
project-3_nlp_naive_bayes
|__ code
|   |__ 01_subreddit_data_collection.ipynb   
|   |__ 02_eda_and_data_cleaning.ipynb   
|   |__ 03a_modeling_naive_bayes.ipynb
|   |__ 03b_modeling_logistic_regression.ipynb 
|   |__ 04a_scattertext_analysis.ipynb
|   |__ 04b_scattertext_analysis_tv_show.ipynb 
|__ data
|   |__ airquality.csv
|   |__ brestcancer.csv
|   |__ thenewsroom.csv
|   |__ thewestwing.csv
|__ project_3_presentation_naive_bayes_nlp.pdf
|__ project_3_presentation_naive_bayes_nlp.pptx
|__ EXECUTIVE_SUMMARY.md 
|__ README.md 
```
