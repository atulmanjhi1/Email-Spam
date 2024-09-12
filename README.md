# Email-Spam

# Spam/Ham Classification using Logistic Regression

This project performs spam/ham classification using Logistic Regression and TF-IDF vectorization.

## Dependencies

The following libraries are required to run this project:
- pandas
- matplotlib
- scikit-learn

## Dataset

The dataset used for this project contains spam and ham (non-spam) text messages. Each message is labeled as either `spam` or `ham`. The dataset includes the following columns:
- `text`: The message content.
- `label_num`: A numerical label where 1 represents spam and 0 represents ham.

## Steps

1. **Data Loading and Preprocessing**
    - The data is loaded using pandas.
    - Unnecessary columns such as `Unnamed: 0` and `label` are removed.
    - The data is split into `X` (text data) and `y` (label data).

2. **Splitting the Data**
    - The dataset is split into training and testing sets using an 80/20 ratio with `train_test_split()`.

3. **Text Vectorization**
    - The text data is converted into numerical format using `TfidfVectorizer`, which transforms the text into TF-IDF vectors.

4. **Model Training**
    - A `LogisticRegression` model is used to train the classifier on the training set.

5. **Prediction**
    - The model is used to predict the labels for the test set.

6. **Evaluation**
    - The model's performance is evaluated using accuracy and classification report metrics.
