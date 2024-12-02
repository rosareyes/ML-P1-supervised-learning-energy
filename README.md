# Machine Learning - Practice 1 
# Supervised Learning for classifying energy

![UC3M Logo](https://assets.onthehub.com/attachments/15/401d138e-5b75-de11-b7f9-0030487d8896/3d13020c-f96c-4a26-8c47-b617961e9c81.jpg)

## Description
This project demonstrates the application of supervised learning techniques for a classification problem. The goal is to classify energy output based on meteorological data from a wind energy dataset. The practice is divided into three stages:

1. **Classification Problem Setup**: Preprocessing the data, engineering features, and transforming the energy prediction problem into a classification task.
2. **Training the Model**: Exploring various supervised learning algorithms, hyperparameter tuning, and evaluating model performance.
3. **Making Predictions**: Using the trained model to generate predictions on a competition dataset and saving results for further use.

## Table of Contents
1. [Introduction](#introduction)
2. [Problem Description](#problem-description)
3. [Dataset](#dataset)
4. [Methodology](#methodology)
   - Data Preprocessing
   - Model Training
   - Model Evaluation
5. [Results](#results)
6. [Files Included](#files-included)
7. [How to Use](#how-to-use)

---

## Introduction
This practice focuses on applying supervised machine learning models to a wind energy dataset. The dataset includes meteorological features and energy production data, with the classification goal of predicting whether energy output is "high" or "low" based on specific thresholds.

---

## Problem Description
The dataset is filtered to focus on Location 13 (`.13` suffix in columns), and energy outputs are categorized into "high" and "low" using the third quartile as the threshold.

---

## Dataset
- **Source**: Wind energy dataset (`wind_ava.csv` and `wind_comp.csv`).
- **Preprocessing Steps**:
  - Filtering for location-specific data.
  - Handling missing values and engineering temporal features (e.g., year, month, day, hour).
  - Classifying energy into two categories.

---

## Methodology

### Data Preprocessing
- Filtered meteorological variables to include only those relevant to Location 13.
- Engineered features such as year, month, and hour from datetime columns.
- Created target labels ("high" or "low") based on energy production thresholds.

### Model Training
- **Algorithms Used**:
  - k-Nearest Neighbors (KNN)
  - Decision Trees
  - Logistic Regression
  - Dummy Classifiers
- Models were trained on a stratified train-test split, with hyperparameter optimization.

### Model Evaluation
- Used metrics such as accuracy, recall, and confusion matrices to evaluate performance.

---

## Results
- k-Nearest Neighbors achieved the best performance among tested models for classification.
- The final model was used to predict energy output categories on a competition dataset.

---

## Files Included
1. `AA2024_G15_P1_clasificacion.ipynb`: Setting up the classification problem.
2. `AA2024_G15_P1_entrenamiento.ipynb`: Training and evaluating models.
3. `AA2024_G15_P1_predicciones.ipynb`: Making predictions with the final model.

---

## How to Use
1. Clone the repository:  
   ```bash
   git clone https://github.com/rosareyes/ML-P1-supervised-learning-energy.git
   cd ML-P1-supervised-learning-energy


