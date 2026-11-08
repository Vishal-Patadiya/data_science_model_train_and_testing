# data_science_model_train_and_testing
```markdown
# Iris Dataset Classification: Random Forest vs. Gaussian Naive Bayes

A comparative machine learning study evaluating the performance of an ensemble decision tree method (**Random Forest**) versus a probabilistic classifier (**Gaussian Naive Bayes**) on the Iris flower dataset.

---

## 📌 Overview

This project benchmarks classification accuracy on the Iris dataset split into designated training and testing subsets. The study examines how non-linear bagging decision boundaries compare against conditional probability models when classifying iris species.

- **Random Forest Classifier**: Achieved **100%** test accuracy.
- **Gaussian Naive Bayes (GaussianNB)**: Achieved **94%** test accuracy.

---

## 📁 Repository Structure

```text
├── first_accuracy_RandomForest.ipynb    # Model training, tuning, and evaluation for Random Forest
├── Second_accuracy_GaussianNB.ipynb     # Model training and evaluation for Gaussian Naive Bayes
├── first.ipynb                          # Exploratory data analysis (EDA) and preliminary prototyping
├── iris_train.xlsx                      # Training dataset
└── iris_test.xlsx                       # Independent test evaluation dataset

```

---

## 📊 Benchmark Results

| Model | Algorithm Type | Test Accuracy | Status |
| --- | --- | --- | --- |
| **Random Forest** | Ensemble (Bagging / Decision Trees) | **100.0%** | Optimal separation |
| **Gaussian Naive Bayes** | Probabilistic (Bayes' Theorem) | **94.0%** | Boundary overlap misclassification |

### Observations

* **Random Forest:** Effectively learned non-linear orthogonal splits across feature dimensions (petal/sepal measurements), classifying all test instances correctly without boundary confusion.
* **Gaussian Naive Bayes:** Exhibited minor misclassifications near the decision boundary between *Iris versicolor* and *Iris virginica*, where feature distributions moderately overlap violating the strict conditional independence assumption.

---

## 🛠️ Requirements & Dependencies

The notebooks require Python 3.8+ and standard scientific computing libraries:

```bash
pip install numpy pandas scikit-learn openpyxl jupyter

```

*(Note: `openpyxl` is required for pandas to read `.xlsx` files)*

---

## 🚀 Getting Started

1. **Clone the repository:**
```bash
git clone [https://github.com/](https://github.com/)<your-username>/<repo-name>.git
cd <repo-name>

```


2. **Launch Jupyter Notebook:**
```bash
jupyter notebook

```


3. **Run the Notebooks:**
* Open `first_accuracy_RandomForest.ipynb` to view the Random Forest workflow and evaluation metrics.
* Open `Second_accuracy_GaussianNB.ipynb` to inspect the Gaussian Naive Bayes model implementation.
* Open `first.ipynb` for initial data exploration and preprocessing checks.



```

```
