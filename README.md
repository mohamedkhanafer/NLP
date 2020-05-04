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

#### Approach I: Basic Processing Methods (stopwords, N-Grams, Mislabeled entries)

#### Approach II: Tokenization, Stemming, Lemmatization and  TF - IDF, POS Tagging

#### Approach III: Better Preprocessing with correction of Spelling Mistakes

#### Approach IV: Simple BERT implementation using the simpletransformers library

___
# 3. Building a Text Summarizer Web Application: Read Smarter, Learn Faster
Based on a survey we conducted on 20 former IE MBA studetnts, we found out that on average, they were assigned 120 cases to read. Out of those, they read only around 58%. And 80% stated that the reason of not reading them was that they were too long or time consuming.

In this group project, we developped a Text Summarizer designed to assist IE MBA students facing this issue. We believe that this Application can be used as an assistant to students, allowing them to summarize online sources and business cases, efficiently saving time in the research and studying stages. 

In order to accomplish this goal, we have analyzed and looked into a set of text summarizers: 

- Four Extractive Summarizers: based on Word Frequency, TF-IDF, Cosine Similarity, and TextRank Algorithm.
- One Abstractive Summarizer: Google's T5 pre-trained Abstractive Summarizer

We used and were inspired by the codes and ideas of [Himanshu Sharma](https://www.presentslide.in/2019/08/text-summarization-python-spacy-library.html), [Jesus Saves](https://jcharistech.wordpress.com/2018/12/31/text-summarization-using-spacy-and-python/), [Akash Panchal](https://towardsdatascience.com/text-summarization-using-tf-idf-e64a0644ace3), [Ashish Singhal](https://medium.com/datapy-ai/nlp-building-text-summarizer-part-1-902fec337b81), [Analytics Vidhya](https://www.analyticsvidhya.com/blog/2018/11/introduction-text-summarization-textrank-python/), [Ramsri Goutham](https://towardsdatascience.com/simple-abstractive-text-summarization-with-pretrained-t5-text-to-text-transfer-transformer-10f6d602c426). For the development of the Web Application, we followed the steps greatly described by [JCharisTech & J-Secur1ty](https://www.youtube.com/watch?v=xvLQdP549NA&t=228s).

This work was done with my study group, comprising namely: Guillermo Chacon, Diego Cuartas, Esteban Delgado, Aayush Kerjiwal, Mariana Naváez, and Valentina Premoli. I here share the Report of our study, the notebook in which we develop the code, the final presentation, and the files that we used to build the Web Application using Flask.

The welcome page allows the user to input the text or the URL containing the article/case/report to summarize:
![WebApp interface](/3_Text_Summarizer_Web_App/webapp.png)

The other page allows to see the output of various summarizers as seen here:
![WebApp interface 2](/3_Text_Summarizer_Web_App/webapp2.png)

