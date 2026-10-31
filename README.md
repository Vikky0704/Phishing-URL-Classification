# Phishing URL Classification Using Machine Learning

**Course:** IAI600 – Group Project

## Project Overview

This project focuses on classifying URLs as legitimate or malicious using machine learning and deep learning techniques.

Two models are developed and evaluated:

- **Hybrid Support Vector Machine (SVM):** Combines character-level TF-IDF features with handcrafted URL features.
- **Character-Level Convolutional Neural Network (CNN):** Uses character-level URL representation to learn patterns for URL classification.

## Dataset

The project uses the prepared dataset:

`phishing_url_dataset_unique.csv`

The target labels are:
- `0` – Legitimate URL
- `1` – Malicious URL

## Models

### 1. Hybrid SVM
- Character-level TF-IDF features
- Handcrafted URL features
- Stratified cross-validation
- GridSearchCV for hyperparameter tuning

### 2. Character-Level CNN
- Text vectorization
- Embedding layer
- Convolutional neural network
- Early stopping during training

## Project Files

| File | Description |
|---|---|
| `phishing_url_project.ipynb` | Main project notebook |
| `phishing_url_dataset_unique.csv` | Prepared dataset |
| `hybrid_svm_model.joblib` | Trained Hybrid SVM model |
| `phishing_url_cnn.keras` | Trained CNN model |
| `phishing_url_vectorizer.joblib` | Saved URL vectorizer |

## How to Use

1. Clone or download this repository.
2. Install the required Python libraries used in the notebook.
3. Open `phishing_url_project.ipynb` in Jupyter Notebook or VS Code.
4. Run the notebook cells in sequence.

## Objective

The objective is to explore and compare machine learning and deep learning approaches for identifying potentially malicious URLs.

---

**Project:** IAI600 Group Project – University West
