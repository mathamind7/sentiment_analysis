# Sentiment Analysis Using Text Preprocessing

This project involves training a sentiment analysis model using a dataset of reviews labeled with sentiments. The pipeline includes data preprocessing, feature extraction using Bag of Words, and model training.

## Dataset
The dataset consists of:
- Original reviews with their corresponding sentiment labels (e.g., positive, negative).

## Data Preprocessing Steps
The following preprocessing steps are applied to prepare the text data for training:

1. **Drop Special Characters**
   - Remove symbols, punctuation, and other non-alphanumeric characters from the text to ensure uniformity.

2. **Convert to Lowercase**
   - Convert all words to lowercase as sentiment analysis is not case-sensitive. This prevents the model from treating words like "Happy" and "happy" differently.

3. **Remove Stopwords and Apply Stemming**
   - Stopwords (e.g., "and", "the", "is") are removed to reduce noise in the data.
   - Words are stemmed to their root forms (e.g., "running" -> "run", "better" -> "good") to group similar terms.

## Feature Extraction: Bag of Words (BoW)
- A Bag of Words model is used to represent the text data numerically.
- Rare tokens that occur infrequently are removed to reduce sparsity and improve model performance.

## Model Training
Once the data is preprocessed and transformed into feature vectors using Bag of Words, the model is trained on this dataset to classify sentiment.

---

### Preprocessing Workflow

1. **Input:** Dataset with original reviews and labels.
2. **Preprocessing Steps:**
   - Clean text by removing special characters.
   - Convert text to lowercase.
   - Remove stopwords and apply stemming.
3. **Feature Engineering:** Create a Bag of Words representation, removing rarely occurring tokens.
4. **Output:** Preprocessed dataset ready for model training.

---

This README provides an overview of the preprocessing pipeline and feature extraction steps for sentiment analysis. You can extend or refine the pipeline based on your project’s specific requirements.

