# CS50 AI Shopping Project

This project implements a k-nearest neighbor classifier to predict whether online shopping customers will complete a purchase based on their browsing behavior.

## Overview

The shopping prediction system analyzes user behavior data including:
- Administrative page visits and duration
- Informational page visits and duration  
- Product-related page visits and duration
- Bounce rates and exit rates
- Page values and special day indicators
- Month, operating system, browser, region, and traffic type
- Visitor type (returning vs new) and weekend indicator

## Implementation

The project uses scikit-learn's KNeighborsClassifier with k=1 to train a model that predicts whether a user will make a purchase (Revenue = True/False).

### Key Functions

- `load_data(filename)`: Loads and preprocesses the CSV data
- `train_model(evidence, labels)`: Trains the k-nearest neighbor classifier
- `evaluate(labels, predictions)`: Calculates sensitivity and specificity metrics

## Usage

```bash
python shopping.py shopping.csv
```

## Results

The model achieves:
- True Positive Rate (Sensitivity): ~40%
- True Negative Rate (Specificity): ~91%

## Data

The dataset contains 12,330 user sessions with 18 features each. The data is from the UCI Machine Learning Repository's "Online Shoppers Purchasing Intention Dataset".

## Author

Yusufbek Abdurakhimov (abduyusufbek.2@gmail.com)
CS50 AI Course Project
