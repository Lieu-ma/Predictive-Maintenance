
# Predictive Maintenance using Machine Learning

![Predictive Maintenance](https://img.shields.io/badge/Predictive-Maintenance-blue)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-orange)
![Python](https://img.shields.io/badge/Python-3.x-green)

This project implements various machine learning models for predictive maintenance using the AI4I 2020 dataset, which simulates predictive maintenance data for industrial equipment.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Models Implemented](#models-implemented)
- [Results](#results)


## Project Overview

Predictive maintenance aims to predict when equipment failures might occur, allowing for timely maintenance and reducing unplanned downtime. This project evaluates multiple machine learning approaches to classify machine failures based on sensor data.

Key aspects:
- Comprehensive data preprocessing and feature engineering
- Handling class imbalance through various techniques
- Evaluation of multiple machine learning models
- Detailed performance metrics and analysis

## Dataset

The AI4I 2020 Predictive Maintenance Dataset contains synthetic data that reflects real predictive maintenance scenarios with the following features:

- Air temperature [K]
- Process temperature [K]
- Rotational speed [rpm]
- Torque [Nm]
- Tool wear [min]
- Machine failure (target variable)
- Failure types (TWF, HDF, PWF, OSF, RNF)

Dataset source: [AI4I 2020 Predictive Maintenance Dataset](https://archive.ics.uci.edu/ml/datasets/AI4I+2020+Predictive+Maintenance+Dataset)

## Features

The project includes:
- Data preprocessing pipeline
- Feature selection and engineering
- Multiple approaches to handle class imbalance:
  - Class weighting
  - SMOTE oversampling
  - Random undersampling
- Model evaluation framework with:
  - Confusion matrices
  - Classification reports
  - Feature importance analysis

## Models Implemented

The following machine learning models were evaluated:

1. **Decision Tree**
   - Weighted version
   - Sampling version

2. **Support Vector Machine (SVM)**
   - Weighted version
   - Sampling version

3. **Random Forest**
   - Weighted version
   - Sampling version

4. **Gaussian Naive Bayes**
   - Standard version
   - Sampling version

5. **Neural Network (MLP Classifier)**

## Results

Key findings from the model evaluations:

- Best recall for failure cases: 94% (Decision Tree with weighting)
- Best precision for failure cases: 46% (SVM with sampling)
- Random Forest with sampling showed balanced performance
- Feature importance analysis revealed torque and rotational speed as most predictive

Detailed results are available in the Jupyter notebook.

