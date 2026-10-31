Phishing URL Classification Using Machine Learning and Deep Learning

Project Overview

This project explores the use of Machine Learning and Deep Learning techniques to classify URLs as Benign or Malicious.

The objective is to investigate how URL characteristics can be used to identify potentially harmful URLs and distinguish them from legitimate URLs.

The project implements and evaluates two approaches:

1. Hybrid Support Vector Machine (SVM): Combines character-level TF-IDF vectorization with 14 manually extracted URL features.
2. Character-Level Convolutional Neural Network (CNN): Uses URL character sequences to learn patterns that help distinguish between benign and malicious URLs.

Models Implemented

1. Hybrid SVM

The Hybrid SVM combines two types of information:

- Character-level TF-IDF features extracted from URLs.
- 14 handcrafted URL features describing URL characteristics.

These features are combined and used to train a Support Vector Machine classifier.

2. Character-Level CNN

The CNN processes URLs as sequences of characters. It learns patterns from the character sequences and uses them to classify URLs.

The model is implemented using TensorFlow and Keras.

Project Workflow

1. Dataset loading and exploration.
2. Data preprocessing and cleaning.
3. Train-test splitting.
4. URL feature engineering.
5. Hybrid SVM model training and evaluation.
6. Character-level CNN model training and evaluation.
7. Model comparison and performance visualization.
8. Saving trained models for future use.

Technologies Used

- Python
- NumPy
- Pandas
- SciPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib
- Joblib

Dataset

The project uses the dataset:

"phishing_url_dataset_unique.csv"

The dataset contains 48,812 records and three columns.

The dataset is required to run the notebook. It is not currently included in the repository, so users must obtain the CSV separately and place it in the project directory.

Note: The project classifies benign and malicious URLs. Malicious URLs are not necessarily all phishing URLs, so the classification terminology should be interpreted accordingly.

Repository Structure

Phishing-URL-Classification/
│
├── README.md
├── phishing_url_project.ipynb
├── hybrid_svm_model.joblib
├── phishing_url_cnn.keras
└── phishing_url_vectorizer.joblib

Installation and Setup

Requirements

- Python 3.14.10
- Jupyter Notebook
- Visual Studio Code with the Jupyter extension

Install the required libraries

python -m pip install numpy pandas scipy scikit-learn matplotlib joblib ipykernel notebook

TensorFlow installation for the Python 3.14 environment:

python -m pip install tensorflow==2.22.0rc0

Running the Project

1. Clone or download this repository.
2. Place "phishing_url_dataset_unique.csv" in the project directory.
3. Open "phishing_url_project.ipynb" in Visual Studio Code.
4. Select the appropriate Python 3.14 kernel.
5. Install the required libraries.
6. Run the notebook cells in sequence.

Saved Model Files

The project includes the following trained artifacts:

File| Description
"hybrid_svm_model.joblib"| Trained Hybrid SVM model
"phishing_url_cnn.keras"| Trained CNN model
"phishing_url_vectorizer.joblib"| Saved TF-IDF vectorizer

Limitations

- The model's performance depends on the quality and diversity of the training dataset.
- Dataset source and label relationships may influence classification results.
- High scores on a random train-test split do not necessarily demonstrate generalization to URLs from previously unseen sources.
- Further testing on independent datasets is needed to assess real-world performance.

Future Work

- Evaluate the models using independent datasets.
- Improve generalization to previously unseen URL sources.
- Explore additional URL features and model architectures.
- Investigate practical deployment for URL classification.

---

Project: Phishing URL Classification Using Machine Learning and Deep Learning
