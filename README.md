
# IMDb Review Sentiment Analysis

This project is a Natural Language Processing (NLP) application that classifies IMDb movie reviews as positive or negative. The classification model leverages various Naive Bayes techniques to determine sentiment, providing valuable insights into audience opinions based on text data.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Information](#dataset-information)
- [Installation](#installation)
- [Data Preprocessing](#data-preprocessing)
- [Model Selection and Evaluation](#model-selection-and-evaluation)
- [Streamlit Deployment](#streamlit-deployment)
- [Results](#results)
- [Future Improvements](#future-improvements)

## Project Overview
The IMDb Sentiment Analysis project classifies text reviews into positive or negative categories. Using various Naive Bayes models—Gaussian, Multinomial, and Bernoulli—we explored the effectiveness of each for text classification. The Multinomial Naive Bayes model was selected for deployment due to its high accuracy on this dataset.

## Dataset Information
- **Volume**: Thousands of IMDb movie reviews.
- **Features**: Text data in the form of user reviews.
- **Labels**: Binary labels (positive or negative) indicating review sentiment.
- The dataset can be downloaded from this link: [IMDb Dataset](https://example.com).

This dataset provides a large volume of text data ideal for training and evaluating a sentiment analysis model.

## Installation
Clone the repository:
```bash
git clone https://github.com/yourusername/imdb-sentiment-analysis.git
cd imdb-sentiment-analysis
```

Install the required libraries:
```bash
pip install -r requirements.txt
```

## Data Preprocessing
Data preprocessing includes:
- **Tokenization**: Breaking down reviews into individual words.
- **Stemming**: Reducing words to their base form for consistency.
- **Vectorization**: Converting text into numerical data using CountVectorizer.

These steps prepare the text data for input into the Naive Bayes models.

## Model Selection and Evaluation
Three Naive Bayes models were trained and evaluated:
1. **Gaussian Naive Bayes**
2. **Multinomial Naive Bayes**
3. **Bernoulli Naive Bayes**

Each model was assessed based on accuracy, with Multinomial Naive Bayes performing the best on this dataset and chosen for deployment. Model accuracy results are as follows:
- **Gaussian**: [78.0]
- **Multinomial**: [85.0]
- **Bernoulli**: [84.0]

## Streamlit Deployment
The Multinomial Naive Bayes model was deployed using Streamlit, providing an interactive interface to test review sentiment predictions in real-time.

To run the Streamlit app:
```bash
streamlit run app.py
```

## Results
The Multinomial Naive Bayes model demonstrated high accuracy, making it effective for classifying IMDb reviews. This model's performance shows potential applications for understanding customer feedback across various domains.

## Future Improvements
Future enhancements could include:
- Exploring other NLP models such as LSTM or BERT for potentially higher accuracy.
- Adding more complex preprocessing steps like stop-word removal and bigram modeling.
- Expanding the dataset to cover a wider range of review topics.
