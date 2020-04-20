# NLP
I here share some codes that I have used during my Natural Language Processing course at IE Univesity. I also share the projects I have done.

# 1. Calculating the Lexical Diversity of songs
I came accross an article discussing the overall vocabulary of some musicians accross their careers. And so I wanted to compare some of the songs of the top 3 artists on that list and the last 2 artists to the 3 songs we saw in class.
On top of the list is (with no surprise) Eminem, which used around 8,800 words in his 100 lenghtiest songs. Then come Jay Z (6,900 words) and Tupac Shakur (6,600 words). On the bottom of the list come the Spice Girls and Bruno Mars (around 1500 words).
I tried to choose songs that seemed more lexically diverse and as expected, the results showed a large diversity difference between the two groups and also when compared to the 3 songs we saw. (the code can be found the the file 1_Lexical_Diversity)
___
# 2. Classification Model: Real or Not? NLP with Disaster Tweets
We are given a dataset of almost 11,000 tweets. The objective is to classify these tweets on whether they are about real disasters or not. The complication comes because many tweets have words that would imply a disaster but are used metaphorically. Therefore, merely identifying the presence of such words would not guarantee that the tweet is in fact referring to an actual disaster.
We have just three pieces of information to do this, the entire actual tweet, the key word in the text and the location from where the tweet has been made.

This is actually an ongoing competition for learning purposes. It is a great one to learn from for anyone interested to explore NLP: https://www.kaggle.com/c/nlp-getting-started. 

This work was done with my colleague Aayush Kejriwal, I here share the code we have written as well as the pdf guide summarizing our thinking. The code is organized as follows:

## A. Problem Description and Dataset
#### A.1 Problem Description and Goal
#### A.2 The Dataset

## B. Exploratory Data Analysis
#### B.1 A general look at the Tweets' text
##### B.1.1 The distributions of the Tweets' Length
##### B.1.2 The distribution of the number of words 
##### B.1.3 Looking at the Stop Words
##### B.1.4 Looking at the most repeated words
#### B.2 The Location of Tweets
#### B.3 The Keywords column 

## C. Building Baseline Models
####  C.1 RidgeClassifier Following Kaggle Tutorial
#### C.2 Multinomial Naive Bayes Classifier
#### C.3 Random Forrest Classifier
#### C.4 Logistic Regression
#### C.5 SVM
#### C.6 Gradient Boosting Classifier
#### C.7 KNN
#### C.8 XGBoost Classifier

## D. Data Cleaning

## E. Approach I: Basic Processing Methods
#### E.1 Removing  stopwords
#### E.2 N-Grams parameter
#### E.3 Mislabeled entries
#### E.4 Using the Keyword column to improve the performance
#### E.5 Conclusion Approach I

## F. Approach II: Tokenization, Stemming, Lemmatization and  TF - IDF
#### F.1 Pre-cleaning
#### F.2 Tokenization, Stemming, and Lematization
#### F.3 Including the keywords into the text
#### F.4 TF - IDF
#### F.5 Running a SVM model with GridSearch
#### F.6 Running a Logistic Regression model with Hyperparameter tunning
#### F.7 Adding the words embeddings
#### F.8 Trying POS Tagging
#### F.9 Discussion: the better approach for considering the Keywords

## G. Approach III: Better Preprocessing with correction of Spelling Mistakes
#### G.1 Running the Correct Spelling Function on the data
#### G.2 Rerunning the models with the correct spelling
##### G.2.1 Model 1 Rerun with spelling corrected

## H. Approach IV: Simple BERT implementation using the simpletransformers library
#### H.1 BERT Model on raw data 
#### H.2 BERT Model on cleaner data 
#### H.3 BERT Model on cleaned and normalized data
#### H.4 BERT Model on cleaned, normalized and relabeled data
#### H.5 BERT Model on data corrected for spelling mistakes
#### H.6 BERT Model on corrected spelling mistakes and normalized data
#### H.7 BERT Model with spelling corrected, with stop words, and lemmatized

## I. Conlusions and Final Model chosen

