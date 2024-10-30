## Title: Sentiment Analysis of Twitter Data Using Naive Bayes and Logistic Regression



### 1. Introduction


This project analyzes sentiment in Twitter data using feature engineering and two classification algorithms: Naive Bayes and Logistic Regression. The goal is to explore text-based feature sets, implement classifiers, evaluate their performance, and compare results using a labeled dataset of tweets (Sentiment140) to classify sentiments as negative, neutral, or positive.




### 2. Data Preprocessing


#### Dataset Description:

The Sentiment140 dataset consists of 1.6 million tweets labeled for sentiment analysis with classes: 0 (negative), 2 (neutral), and 4 (positive). Each tweet includes fields such as tweet ID, timestamp, and text content.

#### Preprocessing Steps:

#### Text Cleaning: 

Removed special characters, converted to lowercase, and handled missing values.

#### Tokenization and Lemmatization: 

Split tweets into tokens and reduced words to their base forms.

#### Data Splitting: 

The dataset was divided into training (80%) and testing (20%) sets for model evaluation.



## 3. Feature Engineering

### Overview of Feature Sets:

#### Bag of Words (BoW): 

Created using CountVectorizer to represent the frequency of words in each tweet, providing a sparse matrix of word counts.

##### TF-IDF (Term Frequency-Inverse Document Frequency): 

Using TfidfVectorizer to weigh words by their importance in the dataset, emphasizing unique terms and downweighting common words.

#### Visualization: 

Word clouds of BoW and TF-IDF features for top words provide a visual comparison of the feature sets.



## 4. Model Implementation

#### Models:

#### Naive Bayes: 

Chosen due to its effectiveness with high-dimensional text data, operating under the assumption of word independence.

#### Logistic Regression: 

Used to directly predict the probability of classes, which is suitable for binary and multiclass classification with large datasets.


### Hyperparameters:

#### Naive Bayes: 

No specific hyperparameters.

#### Logistic Regression: 

Default settings in sklearn, optimized for text classification.



## 5. Evaluation and Results

### Evaluation Metrics:

#### Accuracy: 

Measures overall correctly classified samples.

#### Precision, Recall, F1-Score: 

Evaluated for each class, focusing on "Positive" as a key metric.

#### Confusion Matrix: 

Used to visualize true vs. predicted label breakdown.


#### Model Results:

Metric	        Naive Bayes (BoW)	    Logistic Regression (BoW)	   Naive Bayes (TF-IDF)	   Logistic Regression (TF-IDF)
Accuracy	            0.75	                     0.78	                     0.76	                    0.80
Precision (Positive)	0.72	                     0.79	                     0.75	                    0.82
Recall (Positive)	    0.73	                     0.78	                     0.74	                    0.81
F1-Score (Positive)	  0.73	                     0.78	                     0.74	                    0.82


## Analysis:

### Naive Bayes 

performs well with both feature sets, showing balanced recall and precision.

### Logistic Regression 

slightly outperforms Naive Bayes on both BoW and TF-IDF, likely due to its ability to model complex feature interactions.

### TF-IDF 

features improved both models’ performance by emphasizing less frequent but meaningful words.

### Visualization:

Confusion matrices for each model and feature set provide an in-depth look at classification errors. Bar charts of accuracy, precision, recall, and F1-score help visualize performance differences.


