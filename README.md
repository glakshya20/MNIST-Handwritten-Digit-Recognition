# 🔢 MNIST Handwritten Digit Recognition

A machine learning project that benchmarks multiple classification algorithms on the classic MNIST handwritten digit dataset. Models are compared across different hyperparameter configurations to identify the best performer.

---

## 📌 Overview

This project loads the MNIST dataset (70,000 grayscale 28×28 images of digits 0–9) and trains four different classifiers, each tested with varying hyperparameters. Results are evaluated using accuracy scores and confusion matrices.

---

## 🧠 Models Compared

| Model | Hyperparameters Tested |
|---|---|
| K-Nearest Neighbors (KNN) | k = 3, 5, 7 |
| Support Vector Machine (SVM) | C = 1, 10 (RBF kernel) |
| Logistic Regression | C = 1.0, 0.1 |
| Decision Tree | max_depth = 10, 20 |

---

## 📁 Project Structure

```
├── MNIST_Handwritten_Digit_Recognition.ipynb   # Main notebook
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install numpy matplotlib scikit-learn
```

### Run the Notebook

```bash
jupyter notebook MNIST_Handwritten_Digit_Recognition.ipynb
```

---

## 📊 Dataset

- **Source:** [MNIST via OpenML](https://www.openml.org/d/554)
- **Features:** 784 pixel values (28×28 flattened), normalized to [0, 1]
- **Classes:** Digits 0–9
- **Training subset used:** 10,000 samples
- **Test subset used:** 2,000 samples

---

## 🔍 Workflow

1. **Load & preprocess** — Fetch MNIST from OpenML, normalize pixel values, and split into train/test sets
2. **Train models** — Fit KNN, SVM, Logistic Regression, and Decision Tree with multiple hyperparameter settings
3. **Evaluate** — Print accuracy scores and confusion matrices for each configuration
4. **Predict** — Visualize a sample test image and predict its digit using the best model (SVM, C=10)

---

## 📈 Sample Prediction

```python
# Visualize and predict a single digit
index = 5
plt.imshow(X_test.iloc[index].values.reshape(28, 28), cmap='gray')

svm = SVC(kernel='rbf', C=10)
prediction = svm.predict(X_test.iloc[index].values.reshape(1, -1))
print("Predicted Digit:", prediction[0])
```

---

## 🛠 Tech Stack

- Python 3
- scikit-learn
- NumPy
- Matplotlib
- Jupyter Notebook

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
