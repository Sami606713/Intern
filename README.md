# Spam Email Classifier

This project aims to build a machine learning model for classifying spam and non-spam (ham) emails. The dataset used contains email messages labeled as spam or ham.

## Data Preprocessing

### Shape
- The dataset contains `5572` rows and `2` columns.

### Data Types
- The columns have various data types including strings and numerical values.

### Null Values
- There are no missing values in the dataset.

### Duplicates
- There are `6` duplicated rows in the dataset so we will drop it by using `drop_duplicates() method`.

### Info
- Provides a summary of the dataset including data types and memory usage.

## Text Preprocessing

The text data undergoes several preprocessing steps before modeling:
1. Conversion to lowercase
2. Removal of special characters
3. Tokenization
4. Stemming using the Porter stemming algorithm

## Model Building

A pipeline is constructed comprising text vectorization using TF-IDF and a Bernoulli Naive Bayes classifier. The model is trained on the training data and evaluated on the test data.

### Model Evaluation
- Accuracy Score: ` 0.9737354085603113`
- Confusion Matrix: `[[886   1][ 26 115]]`
- Precision Score: ` 0.9913793103448276`
- Mean Squared Error: `0.026264591439688716`

### Cross-Validation
- Train Score: `0.9742169322962398`
- Test Score: `0.9085389533506986`

## Conclusion

The Bernoulli Naive Bayes model achieved an accuracy of `0.973735` on the test data. Further optimization and exploration of different models may be considered to improve performance.

