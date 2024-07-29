# Sentiment Analysis on Clothing, Shoes, and Jewelry Reviews

This project uses the Clothing, Shoes, and Jewelry dataset to build a model that predicts customer sentiment based on their reviews. The dataset contains reviews and ratings (1-5 stars) which are categorized into sentiment groups. The goal is to classify the sentiment of each review into "like", "dislike", or "neutral" based on the overall rating.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Objectives](#objectives)
- [Installation](#installation)
- [Usage](#usage)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction

The Sentiment Analysis on Clothing, Shoes, and Jewelry Reviews project aims to classify customer feedback into sentiment categories. By analyzing review text and corresponding ratings, the project seeks to understand customer satisfaction and provide insights for improving product offerings.

## Dataset

The dataset used for this project is the Clothing, Shoes, and Jewelry dataset from Amazon reviews, which can be found [here](http://jmcauley.ucsd.edu/data/amazon/).

- **File**: `Clothing_Shoes_and_Jewelry_5.json` (inside `reviews_Clothing_Shoes_and_Jewelry_5.json.gz`)
- **Columns**:
  - `reviewText`: Text of the review.
  - `overall`: Rating given by the customer (1 to 5 stars).

## Objectives

- Predict customer sentiment based on review text.
- Categorize sentiment into three groups:
  - **Like**: 4 or 5 stars.
  - **Dislike**: 1 or 2 stars.
  - **Neutral**: 3 stars.

## Installation

1. Clone the repository:
   ```bash
   git clone [repository_link]
   ```
2. Navigate to the project directory:
   ```bash
   cd sentiment-analysis-clothing
   ```
3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Load and preprocess the dataset:
   ```python
   python data_preprocessing.py
   ```
2. Train the model:
   ```python
   python train_model.py
   ```
3. Evaluate the model:
   ```python
   python evaluate_model.py
   ```

## Modeling

The project employs various machine learning algorithms for sentiment classification, including:

- Naïve Bayes
- Logistic Regression
- Support Vector Machines (SVM)
- Random Forest

## Evaluation

Model performance is evaluated using metrics such as accuracy, precision, recall, and F1-score. The best performing model is selected based on these metrics.

## Conclusion

The project successfully categorizes customer sentiment into like, dislike, and neutral groups, providing valuable insights for understanding customer satisfaction. The model's predictions can help improve product offerings and enhance customer experience.

## References

- [Amazon Product Data](http://jmcauley.ucsd.edu/data/amazon/)
