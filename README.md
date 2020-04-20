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

## B. Exploratory Data Analysis

## C. Building Baseline Models

## D. Data Cleaning

## E. Approach I: Basic Processing Methods (stopwords, N-Grams, Mislabeled entries)

## F. Approach II: Tokenization, Stemming, Lemmatization and  TF - IDF, POS Tagging

## G. Approach III: Better Preprocessing with correction of Spelling Mistakes

## H. Approach IV: Simple BERT implementation using the simpletransformers library

## I. Conlusions and Final Model chosen

