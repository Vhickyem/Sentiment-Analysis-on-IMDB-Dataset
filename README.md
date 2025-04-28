# Sentiment-Analysis-on-IMDB-Dataset

## Overview  
This project focuses on performing sentiment analysis on movie reviews from the IMDB dataset. The goal is to train a model which accurately predict the sentiment (positive or negative) of each review. The dataset, gotten from kaggle consists of 50,000 movie reviews, which are labeled as either positive or negative, making it a binary classification task.

## Purpose  
The primary objective of this project is to analyze the text data from movie reviews and predict the sentiment of the reviews, so as to be able to gain insights into public opinion. In this case, we focus on predicting whether a movie review is positive or negative.

## Dataset  
The dataset used in this project is the IMDB dataset, which consists of 50,000 movie reviews. These reviews are labeled with binary sentiments:

* Positive: The sentiment of the review is favorable towards the movie.

8 Negative: The sentiment of the review is unfavorable towards the movie.

## Project Workflow  
### Data Preprocessing:

* Removal of Duplicates: Duplicates were checked for and 418 rows of duplicate data were removed

* Text cleaning: The reviews are preprocessed by removing html tags, punctuation, and other noise from the text.

* Tokenization: Reviews are tokenized into words to convert them into a format suitable for machine learning models.

* Removal of Stop Words and Lemmatization: Stop words were removed and others were reduced to their base forms, before being joined back as strings

* Vectorization: The tokenized words are converted into numerical features using TF-IDF (Term Frequency-Inverse Document Frequency) technique.

* Model Selection: Various machine learning models were used like Logistic Regression, Support Vector Machine, Random Forest, Naive Bayes and XGBoost

### Model Evaluation:  
After training the models, they are evaluated on the test dataset. Key evaluation metrics such as accuracy, precision, recall, and F1-score are calculated to assess how well the model performs in predicting positive and negative sentiments.

### Results:  
Logistic Regression was the final model chosen because it showed the best performance in classifying sentiment from the movie reviews

Accuracy: 88.6% 

Precision: 90% 

Recall: 87% 

F1-Score: 88% 

### Fine-Tuning  
The final model was fine-tuned, but the accuracy still remained the same.
