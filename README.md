# 🌸 Iris Flower Classification

> Build a machine learning model that classifies an Iris flower into one of three species (*setosa*, *versicolor*, *virginica*) based on four physical measurements.

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Scikit-learn](https://img.shields.io/badge/scikit--learn-1.0+-orange.svg)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📋 Project Overview

This project tackles a classic supervised-learning problem: **multi-class classification** of Iris flowers using their sepal and petal measurements. The Iris dataset is one of the most well-known benchmarks in machine learning and serves as a perfect introduction to the end-to-end ML workflow.

### 🎯 Objectives
- Load and explore the Iris dataset
- Perform exploratory data analysis (EDA) with visualizations
- Preprocess the data (encoding, scaling, train/test split)
- Train and compare **5 classification algorithms**
- Evaluate model performance using accuracy, confusion matrix, and classification report
- Use the best model to make predictions on new flower samples

---

## 📊 Dataset

The Iris dataset contains **150 samples** with **4 features** and **3 balanced classes** (50 samples each).

| Column | Description |
|--------|-------------|
| `SepalLengthCm` | Length of the sepal in centimeters |
| `SepalWidthCm` | Width of the sepal in centimeters |
| `PetalLengthCm` | Length of the petal in centimeters |
| `PetalWidthCm` | Width of the petal in centimeters |
| `Species` | Target class — *Iris-setosa*, *Iris-versicolor*, or *Iris-virginica* |

**Source:** Classic Fisher (1936) Iris dataset — included as `Iris.csv` in this repository.

---

## 🛠️ Tech Stack

- **Python 3.8+**
- **Pandas** & **NumPy** — data manipulation
- **Matplotlib** & **Seaborn** — visualization
- **Scikit-learn** — machine learning models and evaluation
- **Jupyter Notebook** — interactive development

---

## 📁 Repository Structure

```
CodeAlpha_IrisFlowerClassification/
│
├── CodeAlpha_Task1_IrisClassification.ipynb   # Main notebook
├── Iris.csv                                   # Dataset
└── README.md                                  # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

### Run the notebook
```bash
git clone https://github.com/<your-username>/CodeAlpha_IrisFlowerClassification.git
cd CodeAlpha_IrisFlowerClassification
jupyter notebook CodeAlpha_Task1_IrisClassification.ipynb
```

---

## 🔍 Workflow

1. **Data Loading & Exploration** — read the CSV, inspect structure, check for missing values
2. **EDA** — pairplots, boxplots, correlation heatmap to spot class-separating features
3. **Preprocessing** — label encoding for the target, train/test split (80/20, stratified), feature scaling
4. **Model Training** — fit 5 classifiers and evaluate each with 5-fold cross-validation
5. **Model Evaluation** — pick the best model, generate confusion matrix and classification report
6. **Feature Importance** — identify which measurements drive the predictions
7. **Prediction** — classify new, unseen flower samples

---

## 🤖 Models Compared

| Model | Test Accuracy | CV Mean Accuracy |
|-------|:-------------:|:----------------:|
| Support Vector Machine | **96.67%** 🏆 | 96.67% |
| Logistic Regression | 93.33% | 95.83% |
| K-Nearest Neighbors | 93.33% | 96.67% |
| Decision Tree | 93.33% | 94.17% |
| Random Forest | 90.00% | 95.00% |

> 🏆 **Best Model: Support Vector Machine (RBF kernel)** — 96.67% accuracy on the test set.

---

## 📈 Key Findings

- The dataset is **clean, balanced, and small** — ideal for learning the ML workflow.
- **Petal length** and **petal width** are by far the most discriminative features.
- ***Iris-setosa*** is **linearly separable** from the other two species.
- ***Versicolor*** and ***virginica*** show some overlap, accounting for nearly all classification errors.
- All models achieve **≥ 90% accuracy**, demonstrating that the problem is well-suited even to simple algorithms.

---

## 💡 Learning Outcomes

By completing this project I learned to:
- Apply the full supervised-learning workflow: **load → explore → preprocess → train → evaluate → predict**
- Compare multiple classification algorithms objectively
- Use cross-validation to get a robust estimate of model performance
- Interpret confusion matrices and classification reports
- Identify the most important features driving model predictions

## 📜 License

This project is licensed under the MIT License — feel free to use it for learning purposes.

---

⭐ If you found this helpful, please consider giving the repo a star!
