# Vectorization-Techniques-tutorial
Here, various techniques for text embedding are provided to address the problem of predicting the topic of a set of abstracts from two different branches, "Machine Learning in Statistics" and "Applied Statistics," along with their corresponding category labels. Your task is to train a simple classifier that can predict the topic of an article based on its abstract input.

This repository provides a tutorial for those interested in learning about vectorization methods in Natural Language Processing (NLP) using PyTorch and TensorFlow. The majority of the models in this tutorial are implemented with less than 100 lines of code (excluding comments or blank lines).

This code provides a solution to the "Which Statistic?" question in the LLM Hackathon Qualifier. 
: [quera Pages](https://quera.org/problemset/220643)

# NLP students and researchers
Software engineers interested in learning about vectorization methods in NLP
Anyone interested in deep learning and natural language processing
Getting Started:

# To get started, follow these steps:

Clone the repository with the command git clone https://github.com/faezeh-gholamrezaie/Vectorization-Techniques-in-NLP.git

Activate your Python virtual environment.

Install the requirements with the command pip install -r requirements.txt.

Open a Jupyter Notebook in the root directory of the repository.

Run the tutorials and examples in sequence.

# Content:

Tutorials on various common vectorization methods in NLP
Implementations of different NLP models using PyTorch and TensorFlow
Exercises and examples for better understanding of the concepts
Audience.

- [Load Data](#load-data)
- [Preprocess Data](#preprocess-data)
- [Text to Features](#Text-to-Features)
- [Text vectorization](#text-vectorization)
- [Ensemble Models](#Ensemble-Models)

## Load Data

The dataset used in this project is available at the link https://quera.org/contest/assignments/4367/download_problem_initial_project/220643/.
The dataset consists of a number of paper abstracts from two different branches of statistics: "Statistics in Machine Learning" and "Applied Statistics". Each abstract is labeled with its branch.
A simple classifier has been trained to predict the topic of a paper given its abstract.

## Preprocess Data

1. Removing extra white space from text:

All extra white space (more than one space) was removed from the text.
2. Removing all special characters from the text:

All special characters such as periods, commas, question marks, exclamation points, parentheses, etc. were removed from the text.
3. Removing all single characters from the text:

All single characters such as "a", "b", "c", etc. were removed from the text.
4. Converting text to lower case:

All letters in the text were converted to lower case.
5. Word tokenization:

The text was split into separate word tokens.
6. Lemmatization:

All words were converted to their root form.
7. Removing stop words from the text:

Stop words such as "the", "is", "of", etc. were removed from the text.
8. Removing words with a length less than 3 from the text:

All words with a length less than 3 characters were removed from the text.
The purpose of performing these preprocessing steps is to improve the performance of the classification model by removing noise and unnecessary information from the text.

Notes on preprocessing:

The preprocessing steps should be selected based on the type of data and the model being used.

There is no "one size fits all" approach to preprocessing.

It is important to carefully examine the data before selecting the preprocessing steps


## Text to Features

Features are often referred to as independent variables or predictors in machine learning.

Feature Engineering:

In machine learning, features are carefully selected or created from raw data to be most informative for the task at hand. This process is called feature engineering. In text classification, relevant features might include word frequency, document length, or the presence of specific keywords.

## Text vectorization

Text data is inherently different from numerical data that machine learning algorithms typically operate on. Text vectorization techniques aim to bridge this gap by transforming textual data into numerical vectors. These vectors represent the characteristics of the text in a way that can be understood and processed by machine learning models.

There are various techniques for text vectorization, each with its own advantages and limitations. The table below compares the methods used in this project:
[various techniques for text vectorization](https://github.com/faezeh-gholamrezaie/Vectorization-Techniques-in-NLP/blob/main/various%20techniques%20for%20text%20vectorization.png)

## Ensemble Models

We will use three different regression models:

Linear Regression: This is a simple linear model that fits a straight line to the data.

XGBoost: This is a more complex model that uses decision trees to make predictions.

Random Forest: This is a model that uses a large number of decision trees to make predictions.

We will train each of these models on the training data and then average their predictions to make a final prediction. This is known as ensemble averaging and can help to improve the accuracy of our predictions.

# Resources:

Stanford AI Lab - CS224n: Natural Language Processing with Deep Neural Networks: https://nlp.stanford.edu/

Deep Learning for NLP book: https://www.manning.com/books/deep-learning-for-natural-language-processing

PyTorch documentation: https://pytorch.org/docs/

TensorFlow documentation: https://www.tensorflow.org/api_docs
