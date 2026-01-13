# Stellar Object Classification Project

## Overview
This project classifies stellar objects into three categories (**Galaxy, Star, Quasar**) using sensor data. I compared the performance of three models: **LightGBM**, **Random Forest**, and **XGBoost**.

## The Data
* **Source:** [[https://www.kaggle.com/datasets/fedesoriano/stellar-classification-dataset-sdss17]]
* **Size:** 100,000 rows, 17 features (only used 8 features in training).
* **Preprocessing:** Standard Scaling applied; target labels encoded as integers.

## Results & Visualizations

### 1. Model Comparison
Here is the performance comparison across Accuracy, F1, and Precision.

![Model Comparison Graph](plots/Metrics.png) 

### 2. PairPlot
The pairplot for the data.

![Confusion Matrix](plots/pair.png)

## Key Findings
* **LightGBM** achieved the best balance of speed and accuracy.
* **Random Forest** had slightly higher recall and accuracy but was significantly slower to train.
* The "Quasar" class was the hardest to predict due to class imbalance.

## How to Run
1. Clone the repo.
2. Install requirements.
3. Run the notebook: `stellar_classification.ipynb`