# Alphabet Soup Charity Analysis

## Overview

This project focuses on building a neural network model to predict whether organizations funded by Alphabet Soup would be successful. The dataset provided details about past applications, including funding amounts, application types, and classifications.

The main goal was to classify applications as:
- **0**: Unsuccessful (funding was not used effectively)
- **1**: Successful (funding was used effectively)

### Data Information:
- **Target Variable**: `IS_SUCCESSFUL` (success or failure of funding).
- **Features**: Other columns describing the applications.
- **Removed Variables**: `EIN` and `NAME` were removed as they are unique identifiers.

### Machine Learning Process:
The neural network was designed with:
- An input layer and two hidden layers with ReLU activation functions.
- An output layer with a sigmoid activation function for binary classification.

Attempts were made to improve the model's accuracy through various adjustments, such as changing the number of neurons, adding layers, and modifying training parameters.

---

## Results

- **Highest Accuracy Achieved**: **73.2%**
- Despite trying multiple adjustments, the model didn’t meet the target accuracy of 75%. 

---

## Report

For a detailed explanation of the analysis, steps taken, and results, see the full report: [Report.md](./Report.md).
