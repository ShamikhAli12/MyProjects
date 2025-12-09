Project Overview — Multi-Class Sentiment Analysis on Product Reviews
  This project focuses on building a Deep Learning–based sentiment analysis model that predicts product ratings (from 1 to 5 stars) based on customer review text. Unlike simple binary sentiment analysis (positive/negative), this is a multi-class classification problem, where each review is mapped to one of five sentiment levels.

Objective
  Develop a model that can automatically analyze a written review and classify it into:
    1 star → Very Negative
    2 stars → Negative
    3 stars → Neutral
    4 stars → Positive
    5 stars → Very Positive
  This helps in automating customer feedback analysis, improving product insights, and supporting recommendation systems.

Dataset
  The project uses a dataset of product reviews (Reviews.csv), containing:
    Text → The actual customer review
    Score → The rating given by the user (1–5 stars)
  The text data is preprocessed and prepared for neural network training.

Modeling Approach
The workflow includes:
  Text Tokenization & Sequencing -
    Converting review text into numeric sequences using Keras Tokenizer.
  Padding-
    Ensuring all sequences have equal length for model input.
  Deep Learning Model (ANN)-
    A neural network consisting of:
      Embedding layer
      Global Average Pooling
      Dense layers with ReLU
      Softmax output for 5-class classification

  Training & Evaluation:
    The model is trained to learn sentiment patterns and tested on unseen reviews.

Prediction
  Once trained, the model can take any new review and output a predicted rating between 1 and 5, reflecting the sentiment intensity.
