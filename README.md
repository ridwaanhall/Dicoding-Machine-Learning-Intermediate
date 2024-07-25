# Description for LinkedIn Profile**

Developed a comprehensive Google Play Scraper and Sentiment Analysis System for analyzing app reviews, focusing on Mobile Legends and Tokopedia reviews on the Play Store. The project involved several critical steps and components, including:

1. **Google Play Scraper**:
    - Built a custom scraper to fetch app reviews from Google Play Store using the `reviews` function.
    - Implemented pagination handling to fetch large datasets, up to 15,000 reviews, ensuring thorough data collection.
    - Provided functionality to save the scraped reviews into a CSV file for further analysis.

2. **Text Preprocessing**:
    - Designed a series of preprocessing functions for text cleaning, case folding, tokenization, stopword removal, and stemming.
    - Removed mentions, hashtags, retweets, links, numbers, special characters, emojis, and emoticons to clean the text data.
    - Applied Indonesian and English stopwords filtering and custom stopwords removal to refine the text.

3. **Sentiment Analysis Pipeline**:
    - Utilized a pre-trained sentiment analysis pipeline for initial sentiment categorization of the reviews.
    - Processed large batches of data efficiently using the `tqdm` library for progress tracking.

4. **Data Balancing**:
    - Balanced the dataset by resampling to ensure even class distribution for better model performance. Positive, Negative, and Neutral up to 7962*3.

5. **Feature Extraction**:
    - Implemented multiple feature extraction techniques, including TF-IDF, Count Vectorizer, and Word2Vec, to transform text data into numerical features suitable for model training.

6. **Model Training and Evaluation**:
    - Trained several machine learning models, such as Logistic Regression, XGBoost, and Random Forest, using different feature extraction methods and data splits.
    - Achieved high training and testing accuracy, with the best model configuration (Word2Vec and Random Forest) reaching a test accuracy of 98%.

7. **Model Deployment and Inference**:
    - Saved the best-performing model and necessary components (Word2Vec model, Label Encoder) using joblib for deployment.
    - Developed a `SentimentAnalyzer` class to load the models and perform sentiment predictions on new texts.
    - Provided functionality to get detailed sentiment predictions with probability percentages for each class.

8. **Documentation and Results**:
    - Documented the entire process and results, including detailed accuracy scores for different configurations.
    - Presented the sorted results in a clear, readable format to facilitate easy interpretation of the model performance.

This project showcases my ability to handle end-to-end data processing and machine learning pipeline development, from data scraping and preprocessing to model training, evaluation, and deployment. It demonstrates proficiency in Python programming, text processing, and machine learning techniques, with a focus on achieving high accuracy and efficient data handling.
