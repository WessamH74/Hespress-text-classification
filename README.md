# Hespress-text-classification

I have used stories columns to classify each topic, so I have done a lot,
also I have preprocessed data before at EDA repo and saved data to load it for classification.
that's my steps for preprocessing and classification:

1. Removed diacritics (tashkeel).
2. Removed stopwords (في, الى, من).
3. Removed punctuation and special characters (@, #).
4. Used word_tokenize to split text into individual words or tokens.
5. Used ISRIStemmer to perform stemming on tokenized words.
6. Split data into 80% training and 20% testing per class.
7. Split into X_train, Y_train, X_test, Y_test
8. Used TF-IDF to represent the stories and titles as the training features.
9. Defined a linear kernel for SVM and it is considered as binary classification (one vs rest) (ensemble learning).
10. Looped over classes to create a binary classifier for each class to train on it.
11. Looped over classifiers to predict probabilities and determine the class according to the max probability.
12. Evaluated the performance using (accuracy, f1-score, precision, recall) per class.
13. Calculated the confusion matrix.
