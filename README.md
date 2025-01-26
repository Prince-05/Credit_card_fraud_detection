# Credit Card Fraud Detection Using Sampling Techniques

This project focuses on detecting credit card fraud using machine learning models and various sampling techniques to address class imbalance. The primary goal is to accurately classify fraudulent and legitimate transactions by leveraging resampling strategies and comparing the performance of different algorithms.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Techniques Used](#techniques-used)
- [Methodology](#methodology)
- [Results](#results)
- [Requirements](#requirements)
- [Usage](#usage)

## Introduction
Credit card fraud detection is a critical application of machine learning in the financial sector. The dataset used in this project is highly imbalanced, with fraudulent transactions being a small fraction of the total. To address this challenge, the project utilizes:

- Oversampling with SMOTE (Synthetic Minority Over-sampling Technique).
- Random under-sampling for comparison.

## Dataset
The dataset contains the following key attributes:
- Features representing anonymized transaction data.
- A `Class` label, where `0` represents legitimate transactions and `1` represents fraudulent transactions.

## Techniques Used
1. **SMOTE (Synthetic Minority Over-sampling Technique)**: Generates synthetic samples for the minority class to balance the dataset.
2. **Machine Learning Models**:
   - Logistic Regression
   - Decision Tree Classifier
   - Random Forest Classifier
   - Support Vector Machine (SVM)
   - K-Nearest Neighbors (KNN)
3. **Random Sampling**: Generating random subsets of the resampled data for experimentation.

## Methodology
1. **Data Preprocessing**:
   - Load the dataset using pandas.
   - Inspect the dataset for missing values and class distribution.
2. **Resampling**:
   - Apply SMOTE to balance the classes.
   - Compare original and resampled class distributions.
3. **Sampling**:
   - Generate multiple random samples from the resampled data.
4. **Model Training and Evaluation**:
   - Train multiple machine learning models on the samples.
   - Evaluate performance using metrics such as accuracy and F1-score.

## Results
The project highlights the impact of resampling on model performance. It demonstrates how balancing the dataset can improve the detection of fraudulent transactions while maintaining overall accuracy.

## Requirements
To run this project, you need the following Python libraries:
- pandas
- scikit-learn
- imbalanced-learn
- numpy

Install the dependencies using pip:
```bash
pip install pandas scikit-learn imbalanced-learn numpy
```

## Usage
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory and ensure the dataset (`Creditcard_data.csv`) is available.
3. Run the Jupyter Notebook file:
   ```bash
   jupyter notebook SamplingAss1.ipynb
   ```
4. Follow the steps in the notebook to:
   - Load and preprocess the data.
   - Perform resampling and sampling.
   - Train and evaluate models.

## Conclusion
This project demonstrates the effective use of sampling techniques and machine learning algorithms to address the challenge of imbalanced datasets in credit card fraud detection. It serves as a robust foundation for further exploration and optimization of fraud detection systems.

---
For questions or feedback, please feel free to reach out.

