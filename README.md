# Introduction

This project focuses on the **classification of stars** using data from the **Gaia DR3 catalog**, filtered to include stellar properties apparent magnitudes of photometric bands. The goal is to classify stars into their respective spectral types (O, B, A, F, G, K, M) based on these features.

## Project Overview:
We aim to develop a machine learning model capable of accurately classifying stars using their physical characteristics. The dataset includes stars of all spectral types with various features that will be leveraged to train a model and evaluate its performance on unseen data.

## Model Architecture:
For this task, we use a **Artificial Neural Network (ANN)** to handle the classification of stars into spectral types. The ANN is designed to:
- Extract complex patterns from the numerical data (e.g., temperature, luminosity).
- Handle imbalanced classes through techniques such as **SMOTE** to balance the training set.
- Provide robust performance across all spectral classes.

## Task Breakdown:
1. **Data Preprocessing**:
   - Handle missing data by dropping rows or columns and imputing missing values where necessary.
   - Normalize numerical features (e.g. the apparent magnitudes) to ensure uniform scale for model training.
   - Encode the target labels (spectral types) as numerical values.

2. **Balancing the Data**:
   - Use **SMOTE** (Synthetic Minority Over-sampling Technique) to handle class imbalance, ensuring that each spectral type is represented equally in the training data.

3. **Model Training**:
   - Build and train the Artificial Neural Network (ANN) using the preprocessed data.
   - Evaluate the model’s performance using the test set to ensure it generalizes well to unseen data.

4. **Evaluation and Results**:
   - Assess the model’s accuracy, precision, recall, and F1 score to determine its effectiveness in classifying stars into their respective spectral types.
   - Visualize the results using confusion matrices and other metrics.
