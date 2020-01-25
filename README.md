Twitter Sentiment Analysis
==============================

Using Twiiter data to identify the positive and negative sentiments in making a better purchasing decision.

# Project Organization

## Concepts

The following approaches were taken in performing our sentiment analysis through NLP:

- Data Assembly
- Data Processing
- Data Exploration or Visualization
- Model Building & Validation

Let's understand the different data preprocessing activities:

- Convert text to lowercase – Allows us to deal with uniform case text.
- Remove numbers – Numbers usually do not carry any importance in sentiment analysis
- Remove punctuation – For bag of words based sentiment analysis punctuation does not add value.
- Remove stop words – Stop words are common words found in a language and they are mainly neutral.
- Strip white space – Eliminate extra white spaces.
- Tokenization - The process of segmenting running text into words and sentences.
- Lemmatisation – Transform to dictionary base form i.e., “produce” & “produced” become “produce”
- Stemming – Transforms to root word. Stemming uses an algorithm that removes common word endings.

## Exploratory Analysis

I used the following methods to visualize our the tweet field.

- WordCloud: An image that visualizes the unique words extracted from our clean tweet
- ggplot: 
- Frequency Distribution plot: Plots the real frequency of occurrence of text
- Count plot: Plots our categorical data in terms of bars.

## Train-Test Split

I used Scikit-learn's function `train_test_split()`. You need to pass basically 3 parameters features, target, and test_set size. Additionally, I have used random_state to select records randomly.

## Feature Extraction

The features were extracted using two models:

- Bag of Words: A numerical statistic that is intended to reflect the importance of a word in a document from a collection or corpus.
- TF-IDF Features: A numerical statistic that is intended to reflect the importance of a word in a document from a collection or corpus.

## Model Building

I used the following classifiers to build the models:

- Random Forest
- Logistic Regression
- Naive Bayes
- Gradient Boosting

## Evaluation

I used the following metrics to evaluate the performance of our models:

- Accuracy Score: The functions that computes the count of correct predictions.
- Confusion Matrix: A table used to describe the classifier on a set of test data for which the true values are known.
- Classification Report: Measures the quality of our predictions through a classification algorithm through Precision and Recall
