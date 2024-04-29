# Analyzing Spam Collection

This Python script is designed to detect spam messages using a Naive Bayes classifier. It utilizes the natural language processing (NLP) techniques such as bag of words and TF-IDF to preprocess the text data and extract features for classification.

## Dataset
The dataset used for training and testing the classifier is the Spam Collection dataset. It consists of SMS messages labeled as spam or ham (non-spam). The dataset is loaded into a Pandas DataFrame from a CSV file.

## Data Preprocessing
The messages are preprocessed using the following steps:
- Removal of punctuation marks
- Tokenization of text into words
- Removal of stopwords

## Feature Extraction
- Bag of Words (BoW): The text data is transformed into a matrix of word counts using the CountVectorizer from scikit-learn.
- TF-IDF (Term Frequency-Inverse Document Frequency): The BoW matrix is further transformed into a matrix of TF-IDF values to weigh the importance of words in each message.

## Model Training
A Multinomial Naive Bayes classifier is trained on the TF-IDF matrix to classify messages as spam or ham.

## Usage
To use the script:
1. Ensure that all necessary Python libraries are installed (`pandas`, `nltk`, `scikit-learn`).
2. Run the script in a Python environment.

## Results
- The trained model achieves decent accuracy in classifying spam and ham messages.
- The model is evaluated on a subset of the dataset, and the predicted labels are compared with the actual labels.

## Files
- `spam_detection.ipynb`: Jupyter Notebook containing the code.
- `SpamCollection.csv`: Dataset file containing the SMS messages.

---

