# Data Analytics - Level 1 - Task 4: Sentiment Analysis

## Project Overview
This project builds a machine learning model to classify the sentiment of tweets (Positive, Negative, or Neutral) using the Twitter US Airline Sentiment dataset.

## Dataset
- **Name**: Twitter US Airline Sentiment
- **Source**: Kaggle (CrowdFlower)
- **File**: `Tweets.csv`

## Steps Performed

1. **Data Loading & Exploration**
2. **Text Preprocessing**
   - Lowercasing
   - Removal of URLs, mentions, hashtags
   - Stopword removal
   - Lemmatization
3. **Feature Extraction**
   - TF-IDF Vectorizer (max 5000 features)
4. **Model Training**
   - Multinomial Naive Bayes
   - Logistic Regression
5. **Evaluation**
   - Accuracy, Precision, Recall, F1-Score
   - Confusion Matrix
6. **Visualization**
   - Sentiment distribution
   - WordClouds for each sentiment class
7. **Error Analysis**
   - Examined misclassified examples

## Results
- Logistic Regression generally performed better than Naive Bayes.
- The model is more accurate on **Negative** tweets (majority class).
- Suitable for real-world applications such as airline customer service monitoring.

## Tools Used
- Python
- Pandas, NumPy
- Scikit-learn
- NLTK
- Matplotlib, Seaborn
- WordCloud

## How to Run
1. Open `sentiment_analysis.ipynb`
2. Run all cells in order
3. Make sure `Tweets.csv` is in the same folder

## Author
Pranjal Gupta  
Oasis Infobyte Internship – Data Analytics Track
