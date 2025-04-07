## Sentiment Analysis on Customer Reviews (NLP Project)

This project applies Natural Language Processing (NLP) to analyze customer reviews from the Amazon Fine Food Reviews dataset. The objective is to classify reviews as **Positive**, **Negative**, or **Neutral** and derive business insights to understand customer sentiment and improve service quality.

## Project Overview

- Preprocessed thousands of customer reviews using advanced NLP techniques.
- Performed sentiment classification using Logistic Regression and Random Forest.
- Visualized common positive and negative review words using word clouds.
- Evaluated models using accuracy, classification report, and confusion matrix.
- Provided business insights to inform data-driven decision-making.

## Dataset

The dataset used is the **Amazon Fine Food Reviews** containing over 500,000 food-related product reviews, including user ratings and textual comments.

**Features used**:
- `Score`: Rating given by the user (1 to 5)
- `Text`: Review content

[Download Dataset from Kaggle](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews)

## Data Preprocessing

- Removed HTML tags and special characters
- Lowercased all text and removed stopwords
- Tokenized and lemmatized words
- Created new column `clean_text` with preprocessed data
- Mapped scores to sentiments:  
  - 1–2 = Negative  
  - 3 = Neutral  
  - 4–5 = Positive

## Modeling

- Vectorization using **TF-IDF (Unigrams & Bigrams)**
- Handled class imbalance using **RandomUnderSampler**
- Split data into training and test sets
- Used **RandomizedSearchCV** for tuning Logistic Regression
- Trained:
  - Logistic Regression (with hyperparameter tuning)
  - Random Forest Classifier

## Evaluation Metrics

- **Accuracy Scores** for both models
- **Classification Reports**: Precision, Recall, F1-Score
- **Confusion Matrix**: Visual comparison of actual vs predicted labels
- **Word Clouds**: Most frequent positive and negative review words

## Business Insights

- Positive reviews frequently mention words like "love", "great", "delicious".
- Negative reviews highlight issues with "taste", "bad", "disappointed".
- Sentiment models can help companies monitor real-time customer satisfaction.
- Automated analysis saves time and supports customer support teams.

For detailed insights, refer to:  
`insights/Business_Insights_Sentiment_Analysis.docx`

## Conclusion

This project showed how NLP can effectively analyze customer sentiment from textual reviews. Using logistic regression and random forest models, we extracted insights to guide business improvements. Future enhancements could include deep learning models or deployment via web apps.

## Contact

**Author**: Vidhu  
For feedback, collaboration, or queries, feel free to reach out at www.linkedin.com/in/vidhyarajan-mohan-6bb572137.
