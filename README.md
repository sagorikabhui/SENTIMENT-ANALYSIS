# SENTIMENT-ANALYSIS

COMPANY: CODTECH IT SOLUTIONS

NAME: SAGORIKA BHUI

INTERN ID: CITS0D79

DOMAIN: Data Analytics

DURATION: 4 WEEKS

MENTOR: Neela Santhosh

DESCRIPTION:

Project Overview:

This task focuses on performing Sentiment Analysis on social media data using Natural Language Processing (NLP) techniques. The aim is to analyze the sentiments expressed by users in their tweets related to various airlines. By classifying the sentiments as positive, neutral, or negative, we can gain valuable insights into public opinion and customer satisfaction trends. This project demonstrates core concepts of NLP including data preprocessing, feature extraction, model training, and evaluation.

 Dataset Description:

The dataset used in this task is the Twitter US Airline Sentiment dataset, which contains 14 columns and over 14,000 records. Key columns include:

tweet_id: Unique identifier of the tweet.

airline_sentiment: Sentiment label (positive, neutral, or negative).

text: The actual tweet text.

airline: Name of the airline mentioned.

Additional metadata such as tweet location, time, and user info.


This dataset is ideal for sentiment analysis as it contains labeled data from real users expressing opinions about airlines.

 Task Workflow:

Step 1: Data Loading

Using Python’s pandas library, we loaded the CSV file containing the tweets into a DataFrame for easy manipulation and analysis.

 Step 2: Data Exploration

We examined the structure of the dataset, checked for missing values, and analyzed the distribution of sentiments. It was observed that:

Most tweets expressed negative sentiment.

The dataset was imbalanced, with fewer positive and neutral tweets compared to negative ones.

 Step 3: Data Preprocessing

Text data needs to be cleaned before it can be used for model training. We performed:

Removal of usernames (@user), links, special characters.

Lowercasing all text.

Removing stop words (commonly used words that don’t add meaning).

Tokenization and stemming (if needed).


A new column called clean_text was created which stored the preprocessed version of each tweet.

Step 4: Feature Extraction

We used the TF-IDF Vectorizer from the sklearn library to convert the clean text data into numerical features. This allowed us to feed the text into a machine learning model.

Step 5: Model Training

We applied a Logistic Regression classifier to the TF-IDF vectors. The dataset was split into training and testing sets (usually 70:30 or 80:20 split), and the model was trained to predict sentiment labels.

Step 6: Evaluation

After training the model, we evaluated its performance using:

Accuracy Score – percentage of correct predictions.

Classification Report – includes precision, recall, and F1-score for each class.


The final model achieved an accuracy of approximately 81%, which is a strong result considering the class imbalance.

 Key Insights:

Most users expressed negative sentiments, highlighting areas of dissatisfaction with airlines.

The model performed best on the negative class due to its higher representation in the dataset.

Positive and neutral classes were harder to predict due to fewer samples.


 Conclusion:

This task demonstrates how machine learning and NLP techniques can be applied to real-world text data for extracting sentiment insights. Sentiment analysis is a valuable tool for businesses and organizations to monitor public opinion and improve their services based on customer feedback. The successful implementation of this task reflects practical skills in data cleaning, feature engineering, and text classification using Python.
