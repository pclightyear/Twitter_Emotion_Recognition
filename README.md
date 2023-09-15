# Emotion Recognition on Twitter

The goal of this project is to predict the emotion behind the tweets. This is a [competition](https://www.kaggle.com/competitions/dm19-lab2-nthu/overview) from the data mining course offered in Nation Tsing Hua University.

We preprocess the tweets and trained a LSTM model on 1.46 million tweets. Our method reaches 0.477 mean f1-score on testing data and places 9th out of 40 teams in the class. The complete report is provided in [this notebook](https://github.com/pclightyear/Twitter_Emotion_Recognition/blob/master/Part3_Report.ipynb).

## Preprocessing
- Replace tokens in the dataset such as "@user" and hashtag into tokens in the dictionary of the pre-trained embeddings.
- Replace common emojis to their corresponding adjectives.

## Training
- Convert the tweets into glove embeddings.
- Train a LSTM model to predict the emotion behind the tweets.
- Validation set is used to prevent overfitting.

## Data
- Training set - 1.46m tweets
- Testing set - 412k tweets

There are 8 different emotion labels in the dataset: anger, anticipation, disgust, fear, sadness, surprise, trust, and joy.

Follow the [link](https://www.kaggle.com/competitions/dm19-lab2-nthu/data) to download the dataset.

## Tools in use
- keras
- nltk
- scikit-learn
