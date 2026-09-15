# Sentiment Analysis of Amazon Product Reviews

## 📌 Project Overview

This project focuses on analyzing customer opinions from Amazon product reviews using Natural Language Processing (NLP) and Machine Learning techniques. The main objective is to classify customer reviews into positive, neutral, or negative sentiments and detect the emotions expressed in the text to better understand customer satisfaction and improve the shopping experience.

## 🎯 Objectives

* Analyze customer opinions and feedback from Amazon product reviews.
* Clean and preprocess textual data.
* Explore sentiment distributions and review characteristics.
* Compare different text representation techniques.
* Build a sentiment classification model using Logistic Regression.
* Detect emotions expressed in customer reviews using a pretrained RoBERTa model.

## 📂 Dataset

The project uses an Amazon product reviews dataset containing customer comments and ratings.

The main columns used in the analysis are:

* **Comment:** Customer review text.
* **Rating:** Product rating provided by the customer.

Sentiment labels are assigned according to the rating:

| Rating | Sentiment |
| ------ | --------- |
| 4–5    | Positive  |
| 3      | Neutral   |
| 1–2    | Negative  |

## 🧹 Data Cleaning and Exploratory Data Analysis

The preprocessing and exploration steps include:

* Selecting the review and rating columns.
* Removing missing values.
* Cleaning reviews by removing stopwords and punctuation.
* Assigning sentiment labels based on ratings.
* Analyzing the distribution of sentiment categories.
* Studying review length and the most frequent words in negative reviews.

## 🤖 Machine Learning

A Logistic Regression classifier is used to predict the sentiment of customer reviews.

The following text representation techniques are compared:

* Count Vectorization
* TF-IDF Word
* TF-IDF N-grams
* TF-IDF Characters

### Model Performance

| Text Representation | Accuracy |
| ------------------- | -------: |
| Count Vectors       |    80.3% |
| TF-IDF Word         |    77.3% |
| TF-IDF N-grams      |    75.9% |
| TF-IDF Characters   |    76.8% |

Among the evaluated approaches, Count Vectorization achieved the highest accuracy of 80.3% on the reported evaluation.

## 😊 Emotion Detection

To complement sentiment classification, the project uses the **RoBERTa-base-GoEmotions** model from Hugging Face Transformers.

The model is trained on the GoEmotions dataset and can identify 28 different emotion categories. For each review, the two emotions with the highest predicted scores are selected for analysis.

This approach helps provide a more detailed understanding of customer feedback beyond positive, neutral, and negative sentiment labels.

## 🛠️ Technologies Used

* Python
* Natural Language Processing (NLP)
* Machine Learning
* Logistic Regression
* Count Vectorization
* TF-IDF
* Hugging Face Transformers
* RoBERTa
* GoEmotions
* Pandas
* NumPy
* Matplotlib
* Seaborn

## 📊 Key Outcomes

This project demonstrates how NLP and Machine Learning can be applied to customer reviews to:

* Classify customer sentiment.
* Identify patterns in customer feedback.
* Detect emotions expressed in reviews.
* Support businesses in understanding customer satisfaction and identifying areas for improvement.



**Program:** M2 Data Science for Business (DSB)
