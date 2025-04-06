# Secom_semi-conductor_manufacturing
This repository presents a comprehensive analysis of the SECOM dataset, which originates from a real-world semiconductor manufacturing process. The goal is to identify critical signals from a high-dimensional dataset to improve the predictability of product yield outcomes.

In high-tech production environments, countless variables are measured from sensors and process checkpoints. However, only a subset of these signals are truly useful for quality control and defect prediction. Through intelligent feature selection and robust modeling, this project aims to streamline variable analysis and support data-driven process improvements.

## Project Overview

The dataset contains **1567 samples** and **591 features**, along with a corresponding binary classification label indicating pass/fail status at an internal testing point. The class labels are encoded as -1 for pass and 1 for fail. 

Notable challenges in the data include:
- Missing values (`NaN`)
- Redundant or low-variance features
- Highly imbalanced class distribution

### Objectives:
- Identify informative signals that influence yield
- Improve classification accuracy using preprocessing and modeling
- Enhance interpretability through feature ranking and visualization

## Key Highlights

- Real industrial dataset with high-dimensional, noisy data
- Feature selection using correlation filtering, and RFE
- Preprocessing pipelines for missing value imputation, scaling, and outlier detection
- Handling imbalanced classes using sampling techniques
- Model evaluation through cross-validation and multiple performance metrics
- Final models include Logistic Regression, Random Forest, SVM, KNN, and XGBoost
- Visual tools: confusion matrices, ROC curves, PR curves

## Data Structure

- `SECOM Data File`: 1567 samples × 591 features (sensor/process measurements)
- `Labels File`: Contains pass/fail outcome (-1/1) and associated timestamps

## Methodology (CRISP-DM Framework)

1. **Business Understanding** – Understand yield loss and quality control costs
2. **Data Understanding** – Assess distributions, volatility, and missingness
3. **Data Preparation** – Clean, impute, scale, and reduce features
4. **Modeling** – Fit ML models and fine-tune parameters
5. **Evaluation** – Compare models using metrics like accuracy, F1-score, and AUC
6. **Deployment** – Interpret top features and model outputs


