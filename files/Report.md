# Alphabet Soup Charity Analysis Report

---

## Overview of the Analysis

The purpose of this analysis was to create a deep learning model to predict whether organizations funded by Alphabet Soup would be successful. The dataset included details about each application, and the goal was to train a binary classification model that could accurately determine whether funding would lead to success (`1`) or not (`0`).

---

## Results

### Data Preprocessing

- **Target Variable**: 
  - `IS_SUCCESSFUL` (indicates whether funding was used effectively).
- **Feature Variables**: 
  - Columns such as `APPLICATION_TYPE`, `CLASSIFICATION`, `ASK_AMT`, and others that describe the applications.
- **Removed Variables**: 
  - `EIN` and `NAME` were removed because they are unique identifiers and not useful for prediction.

---

### Compiling, Training, and Evaluating the Model

- **Neurons, Layers, and Activation Functions**:
  - Initially, the model had two hidden layers with **80 neurons in the first layer** and **30 neurons in the second**, both using the **ReLU activation function**.
  - Later, more neurons were added (**100 in the first layer, 50 in the second**) and a **third hidden layer with 25 neurons** was introduced. The output layer used a **sigmoid activation function** for binary classification.

- **Target Performance**:
  - The highest accuracy achieved was **73.2%**, which did not meet the target of **75%**.

- **Steps Taken to Improve Performance**:
  1. **Increased neurons** in the layers to make the model more powerful.
  2. **Added a third hidden layer** to introduce more complexity.
  3. **Trained for more epochs** (up to 100) to give the model more time to learn.
  4. **Reduced batch size** to 16 for finer weight updates during training.
  5. **Added dropout layers** to prevent overfitting, although this resulted in lower accuracy.

---

## Summary

The best accuracy achieved was **73.2%**, which fell short of the target of **75%**. While various optimizations were attempted, including changes to the model architecture, training parameters, and data preprocessing, the accuracy improvements were minimal.

### Recommendation
If I had more time, I would:
- Experiment further with the number of neurons and layers to find a better balance.
- Focus on simplifying or refining the data further to help the model learn better patterns.
- Consider trying different activation functions to see if they improve performance.

Even though the target was not reached, this project provided valuable experience in testing, optimizing, and analyzing deep learning models.
