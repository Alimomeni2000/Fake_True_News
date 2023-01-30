# [Fake_True_News](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)

### 0. Introduction

In this notebook, we are going to be building a Neural Language Model to classify news as being fake or real. We will start off by loading in the required libraries, and importing the data. Then we will clean the data to remove any obvious differences between the fake and real articles. Finally we will adapt a pre-trained BERT model for it to be able to classify between the fake and real articles.


### 1. Data

The data consists of 23481 fake and 21417 real news articles (source: www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset). The real articles were originally obtained by scraping articles from Reuters.com. The Fake articles were obtained from websites that were flagged by a fact-checking website (Politifact) and Wikipedia. The real articles were all published between the 13th of January 2016 and the 31th of December 2017. The fake articles were published between the 31th of March 2015 and the 19th of February 2018.


### 2. Research Question

We are mainly interested in finding out how well modern NLP models can distinguish between real and fake articles. Defining what is fake or real news can be tricky however, and we expect that our data will reflect this. Therefore, we are also interested in finding various characteristics in our fake and real articles that might lead to overfitting.
