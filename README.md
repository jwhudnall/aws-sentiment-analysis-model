# SageMaker Deployment Project

The notebook and Python files provided here, once completed, result in a simple web app which interacts with a deployed recurrent neural network performing sentiment analysis on movie reviews. This project assumes some familiarity with SageMaker, the mini-project, Sentiment Analysis using XGBoost, should provide enough background.

Please see the [README](https://github.com/udacity/sagemaker-deployment/tree/master/README.md) in the root directory for instructions on setting up a SageMaker notebook and downloading the project files (as well as the other notebooks).

**Personal Note:** 
This project serves a sentiment analysis machine learning model to users via a very basic web app. After a user types in a review, the model predicts whether the sentiment was positive or negative.

Under the hood, past IMDB movie review data is preprocessed and tokenized using nltk, numpy and custom python functions. The data is then split into train/test sets, trained via a recurrent neural network in AWS SageMaker, and tested for accuracy. Once the model performs acceptably, it is deployed to an AWS endpoint for use.
