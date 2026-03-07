# 🔢 MNIST Handwritten Digit Recognition

A Convolutional Neural Network (CNN) model trained on the MNIST dataset to classify handwritten digits (0–9) with high accuracy.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

---

## 📌 Overview

This project uses deep learning to recognize handwritten digits from images. The model is trained on the classic MNIST dataset containing 70,000 grayscale images (28×28 pixels) across 10 classes.

**Model Accuracy:** ~99% on the test set

---

## 🧠 Tech Stack

- **Python** — Core language
- **TensorFlow / Keras** — Model building & training
- **NumPy / Matplotlib** — Data processing & visualization
- **Jupyter Notebook** — Interactive development

---

## 🗂️ Project Structure

```
MNIST-Handwritten-Digit-Recognition/
│
├── mnist_model.ipynb      # Main notebook: EDA, model training, evaluation
├── README.md
```

---

## 🚀 How to Run

### 1. Clone the repo
```bash
git clone https://github.com/glakshya20/MNIST-Handwritten-Digit-Recognition.git
cd MNIST-Handwritten-Digit-Recognition
```

### 2. Install dependencies
```bash
pip install tensorflow numpy matplotlib jupyter
```

### 3. Launch the notebook
```bash
jupyter notebook mnist_model.ipynb
```

---

## 📊 Results

| Metric | Value |
|--------|-------|
| Training Accuracy | ~99% |
| Test Accuracy | ~98.9% |
| Epochs | 10 |
| Optimizer | Adam |

---

## 📚 What I Learned

- Building and training CNNs with Keras
- Understanding convolution, pooling, and flatten layers
- Visualizing model performance with confusion matrices
- Importance of data normalization in ML pipelines

---

## 🔮 Future Improvements

- [ ] Add a Flask web interface where users can draw a digit and get a live prediction
- [ ] Experiment with data augmentation to push accuracy further
- [ ] Export model as `.h5` and deploy on Hugging Face Spaces

---

## 👤 Author

**Lakshya Gupta** — [LinkedIn](https://www.linkedin.com/in/lakshya-gupta7/) | [GitHub](https://github.com/glakshya20)
