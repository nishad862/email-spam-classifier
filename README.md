# email-spam-classifier

# Problem Statement
Spam messages are a common issue in digital communication, leading to wasted time and potential security risks.
This project aims to automatically detect spam messages using text preprocessing, TF-IDF vectorization, and supervised machine learning.


# Tech Stack
Programming Language: Python
Machine Learning: Scikit-learn
NLP: NLTK
Model: Multinomial Naive Bayes
Vectorization: TF-IDF
Web Framework: Streamlit
Deployment: Streamlit Community Cloud


# Project Workflow
-Data Cleaning
    Removed unnecessary columns
    Removed duplicate messages
    Label encoded target variable (Spam / Ham)
-Exploratory Data Analysis
    Message length analysis
    Word & sentence distribution
    Spam vs Ham comparison
-Text Preprocessing
    Lowercasing
    Tokenization
    Removing stopwords & punctuation
    Stemming using Porter Stemmer
-Feature Engineering
    TF-IDF Vectorization (max_features = 3000)
-Model Training & Evaluation
    Tried multiple ML models
    Selected Multinomial Naive Bayes for best precision
-Deployment
    Built an interactive web app using Streamlit
    Deployed on Streamlit Community Cloud


# Model Performance
Metric	Score
Accuracy	~97%
Precision	~100%
Precision was prioritized to minimize false positives (i.e., misclassifying genuine messages as spam).


# Application Preview
Link to the application : https://sms-spam-classifier8625.streamlit.app
Steps to use the app:
Enter an email or SMS message
Click Predict
Instantly see whether the message is Spam or Not Spam


# How to Run Locally
1) Clone the repository
    git clone https://github.com/YOUR_USERNAME/email-spam-classifier.git
    cd email-spam-classifier
2) Install dependencies
    pip install -r requirements.txt
3) Run the app
    streamlit run app.py
