# Loan Approval Prediction using Artificial Neural Network (ANN)

## Project Overview

This project uses an Artificial Neural Network (ANN) to predict whether a loan application will be **Approved** or **Rejected** based on applicant information such as income, loan amount, CIBIL score, assets, education, and employment status.

The model was built using TensorFlow/Keras and evaluated using standard classification metrics.

---

## Dataset Information

Dataset: Loan Approval Dataset

Total Records: 4,269

Features:

- no_of_dependents
- education
- self_employed
- income_annum
- loan_amount
- loan_term
- cibil_score
- residential_assets_value
- commercial_assets_value
- luxury_assets_value
- bank_asset_value

Target Variable:

- loan_status
  - Approved = 1
  - Rejected = 0

---

## Data Preprocessing

The following preprocessing steps were performed:

1. Dataset loading using Pandas
2. Missing value inspection
3. Column name cleaning
4. Categorical value cleaning
5. Label encoding of categorical features
6. Removal of loan_id column
7. Feature scaling using StandardScaler
8. Train-Test Split (80% Training, 20% Testing)

---

## ANN Architecture

Input Layer:
- 11 Features

Hidden Layer 1:
- 16 Neurons
- ReLU Activation

Hidden Layer 2:
- 8 Neurons
- ReLU Activation

Output Layer:
- 1 Neuron
- Sigmoid Activation

Optimizer:
- Adam

Loss Function:
- Binary Crossentropy

Epochs:
- 20

Batch Size:
- 32

---

## Model Performance

### Test Results

| Metric | Value |
|----------|----------|
| Accuracy | 94.15% |
| Precision | 95.17% |
| Recall | 95.52% |

### Classification Report

| Class | Precision | Recall | F1-Score |
|---------|---------|---------|---------|
| Rejected (0) | 0.92 | 0.92 | 0.92 |
| Approved (1) | 0.95 | 0.96 | 0.95 |

---

## Files Included

- ANN - Loan Approval Prediction (Binary Classification).ipynb
- loan_approval_dataset.csv
- trained_model.h5
- scaler.pkl

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- TensorFlow / Keras
- Jupyter Notebook

---

## Author

Noman

ANN Assignment – Loan Approval Prediction (Binary Classification)
