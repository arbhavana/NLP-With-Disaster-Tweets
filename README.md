# NLP-With-Disaster-Tweets

# Disaster Tweet Classification

This project aims to classify tweets related to disasters as either disaster-related or not. The model uses Natural Language Processing (NLP) techniques, including word embeddings, to predict whether a tweet is indicative of a real disaster event.

## Overview
This project involves the use of machine learning models and NLP techniques to classify tweets into two categories: disaster-related and not disaster-related. The model was trained on a dataset of tweets and achieves a certain level of accuracy based on the training process.

## Dataset
The dataset used for this project comes from Kaggle. It contains labeled tweets with binary outcomes: `1` for disaster and `0` for non-disaster. The tweets are labelled manually.


## Approach
1. **Data Preprocessing**:
    - Removed irrelevant characters, URLs, and special symbols.
    - Tokenization of text and lowercasing.
    - Removal of stopwords and lemmatization.

2. **Feature Engineering**:
    - Word Embeddings using pre-trained models like Word2Vec, GloVe, or FastText.
    - Represented tweets as dense vectors for better classification.

3. **Modeling**:
    - Various machine learning models were trained, including Logistic Regression, Support Vector Machines (SVM), and Random Forest algorithms.

## Model and Techniques
- **NLP Techniques**: Word embeddings, tokenization, stopword removal, and lemmatization.
- **Machine Learning Models**: 
    - Logistic Regression
    - Support Vector Machine (SVM)
    -  Random Forest.


### Real-Time Tweet Fetching and Visualization

This project features real-time tweet fetching using the **Twitter API**. By obtaining a Bearer Token from Twitter's Developer platform, we can stream tweets in real-time.

#### Key Components:

1. **Bearer Token Authentication**: 
   The Bearer Token, obtained from the Twitter Developer portal, is used to authenticate requests to the Twitter API. This allows continuous access to Twitter’s streaming API, which listens for tweets that match the predefined disaster-related keywords.

2. **Real-Time Data Fetching**:
   Tweets are fetched in real-time by connecting to the Twitter streaming API. The data is filtered based on keywords relevant to the disaster domain. This allows us to gather fresh, real-time insights about disaster events as they are discussed on social media.

3. **Visualizing Tweets with Streamlit**:
   Streamlit is used to create a user-friendly web interface that displays the fetched tweets in real-time. The interface allows for dynamic updating as new tweets are streamed.

4. **Using ngrok for Public Access**:
   Since the Streamlit app runs locally, **ngrok** is utilized to expose the local application to the internet. This creates a public URL that can be shared with others, making the real-time tweet stream accessible from anywhere.

