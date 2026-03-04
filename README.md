# Credit Risk Prediction using Multi-Layer Perceptron (MLP)

## Project Overview

This project implements a **Neural Network based credit risk prediction system** using a **Multi-Layer Perceptron (MLP)**.
The model is trained on a tabular credit dataset to classify customers into **low risk or high risk categories**.

The purpose of this project is to understand the working of **feedforward neural networks, activation functions, loss functions, and model evaluation techniques** as part of a Deep Learning laboratory assignment.

---

## Dataset

The dataset used is the **German Credit Dataset**.

It contains financial and demographic information about loan applicants, including:

* Age
* Sex
* Job
* Housing
* Saving accounts
* Checking account
* Credit amount
* Loan duration
* Loan purpose

These features are used to predict the **credit risk level**.

---

## Data Preprocessing

The following preprocessing steps were performed:

1. Removed unnecessary columns.
2. Handled missing values in categorical columns.
3. Encoded categorical variables using **Label Encoding**.
4. Normalized numerical features using **StandardScaler**.
5. Split the dataset into **training and testing sets (80/20)**.

---

## Model Architecture

A **Multi-Layer Perceptron (MLP)** neural network was implemented with the following architecture:

| Layer          | Neurons            | Activation |
| -------------- | ------------------ | ---------- |
| Input Layer    | Number of features | —          |
| Hidden Layer 1 | 32                 | ReLU       |
| Hidden Layer 2 | 16                 | ReLU       |
| Output Layer   | 1                  | Sigmoid    |

Loss Function: **Binary Crossentropy**
Optimizer: **Adam**

---

## Training

The model was trained using:

* **Epochs:** 30
* **Batch Size:** 32
* **Validation Split:** 20%

Training and validation metrics were recorded to monitor model performance.

---

## Evaluation Metrics

The model performance was evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

These metrics help assess how well the model predicts credit risk.

---

## Tools and Libraries

The project was implemented using the following Python libraries:

* TensorFlow / Keras
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

---

## Project Structure

```
credit-risk-mlp
│
├── german_credit_data.csv
├── credit_risk_model.ipynb
└── README.md
```

---

## How to Run the Project

1. Clone the repository

```
git clone https://github.com/King87429/credit-risk-mlp.git
```

2. Navigate to the project directory

```
cd credit-risk-mlp
```

3. Install required libraries

```
pip install pandas numpy scikit-learn tensorflow matplotlib seaborn
```

4. Run the notebook

```
credit_risk_model.ipynb
```

---

## Conclusion

This project demonstrates how neural networks can be applied to **credit risk prediction problems** using structured data. The Multi-Layer Perceptron successfully learns patterns in financial attributes and predicts credit risk categories.
