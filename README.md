## Sentiment Analysis on Twitter Data Using Naive Bayes and Logistic Regression



### Project Overview

This project implements Naive Bayes and Logistic Regression classifiers on the Sentiment140 dataset to analyze tweet sentiment. 
Feature engineering methods include Bag of Words (BoW) and TF-IDF representations.


### Prerequisites

Ensure Python 3.6+ is installed. Use pip to install dependencies.


### Dependencies

Install the following packages using the command below:

## pip install pandas scikit-learn matplotlib seaborn nltk


### pandas: 

For data manipulation.


### scikit-learn: 

For machine learning models and metrics.


### matplotlib & seaborn: 

For visualizations.


### nltk: 

For text preprocessing, tokenization, and lemmatization.


## Dataset

Download the Sentiment140 dataset from Kaggle and save it as training.1600000.processed.noemoticon.csv in the project folder.

### Instructions


#### Preprocess Data: 

The code will automatically preprocess text by removing special characters, converting to lowercase, tokenizing, and lemmatizing.
Feature Engineering: The script generates BoW and TF-IDF feature sets.


#### Model Training and Evaluation:


The Naive Bayes and Logistic Regression models are trained, evaluated, and compared based on accuracy, precision, recall, and F1-score.


### How to Run the Code

Place the Sentiment140 dataset file in the project directory.

Execute the script

### python sentiment_analysis.py

This will:

Preprocess data.

Generate feature sets.

Train and evaluate both models.


### Results: 

The script will output a performance summary table and save visualizations in the results folder.
