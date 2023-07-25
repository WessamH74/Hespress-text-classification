# Hespress-text-classification

I have used stories and title columns to classify each topic,
also I have preprocessed data before at the EDA repo and saved data to load it for classification.
that's my steps for preprocessing and classification:

1. Removed diacritics (tashkeel).
2. Removed stopwords (في, الى, من).
3. Removed punctuation and special characters (@, #).
4. Used word_tokenize to split the text into individual words or tokens.
5. Used ISRIStemmer to perform stemming on tokenized words.
6. Split data into 80% training and 20% testing per class.
7. Split into X_train, Y_train, X_test, Y_test
8. Used TF-IDF to represent the stories and titles as the training features.
9. Uses Naive Bayes classifier with GridSearch cross-validation to find best parameters
10. Naive Bayes had a 78% accuracy
11. Trained another model support vector machine with linear kernel, also I applied GridSearch cross-validation to find the best parameters
12. SVM had 85% accuracy
13. Evaluated the performance using (accuracy, f1-score, precision, and recall) per class for the 2 classifiers.
14. Calculated the confusion matrix for the best classifier (SVM).
