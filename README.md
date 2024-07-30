# Internship_task_1
## Sentiment Analysis on Tweets

This repository contains a machine learning pipeline for sentiment analysis on tweets. The project utilizes various text preprocessing techniques, feature extraction methods, and classification algorithms to classify tweets as either positive or negative.

## Project Overview

The primary goal of this project is to build and evaluate a sentiment analysis model using Logistic Regression. The model is trained on a balanced dataset of tweets and can predict the sentiment of new, unseen text.

## Dataset

The dataset used for training and evaluation is a collection of tweets from the [Sentiment140](http://help.sentiment140.com/for-students) dataset. The dataset includes:

- `target`: Sentiment label (0 for negative, 1 for positive)
- `ids`: Tweet ID
- `date`: Tweet date
- `flag`: Query flag
- `user`: Username
- `text`: Tweet text

The dataset is loaded from a CSV file, `training.1600000.processed.noemoticon.csv`.

## Setup

### Prerequisites

- Python 3.x
- Libraries:
  - `numpy`
  - `pandas`
  - `seaborn`
  - `matplotlib`
  - `nltk`
  - `scikit-learn`
  - `wordcloud`
  - `google.colab` (for Google Colab users)

### Installation

1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```
   
2. **Install required libraries:**

       pip install numpy pandas seaborn matplotlib nltk scikit-learn wordcloud

3. **Download the dataset:**
   
Place the training.1600000.processed.noemoticon.csv file in the appropriate directory or update the path in the code to the location of the dataset file on your local machine.
  

### Usage
Run the Jupyter Notebook or Python Script:
Execute the code to perform the following tasks:

* Load and preprocess the dataset.
* Visualize the data distribution and word clouds.
* Train and evaluate a Logistic Regression model.
* Predict sentiment for new text inputs.

**Sentiment Prediction:**
Use the predict_sentiment(sentence) function to predict the sentiment of a new tweet.

    sentence = 'Wow you guys have done a fantastic job! Keep it up!'
    sentiment = predict_sentiment(sentence)
    print(sentiment)
    
    
    sentence = 'Really bad! Never expected such work from you! Try to improve the quality and service.'
    sentiment = predict_sentiment(sentence)
    print(sentiment)
    

### License
This project is licensed under the MIT License. See the LICENSE file for details.

### Acknowledgements
The Sentiment140 dataset used for training and evaluation.
NLTK and Scikit-learn libraries for text processing and machine learning functionalities.
