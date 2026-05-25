# MNIST Handwritten Digit Recognition Using Deep Learning

## 🎯 Objective
Build a Neural Network that can look at a handwritten digit image 
and accurately predict which number (0–9) it represents.

---

## 📊 Dataset
**MNIST Dataset** — one of the most well-known datasets in Machine Learning.

| Property | Detail |
|----------|--------|
| Source | TensorFlow built-in (`tf.keras.datasets.mnist`) |
| Total Images | 70,000 handwritten digit images |
| Image Size | 28 × 28 pixels |
| Classes | 10 (digits 0 to 9) |
| Train Set | 60,000 images |
| Test Set | 10,000 images |

---

## 🧠 Model Architecture

| Layer | Details |
|-------|---------|
| Input | 28×28 image |
| Flatten | Converts 2D image → 1D array (784 values) |
| Dense | 128 neurons, ReLU activation |
| Dropout | 20% — prevents overfitting |
| Output | 10 neurons (one per digit class) |

---

## ⚙️ Tech Stack
- Python
- TensorFlow / Keras
- NumPy
- Google Colab

---

## 📈 Results

| Metric | Score |
|--------|-------|
| Training Accuracy | 95.30% |
| Test Accuracy | **96.46%** ✅ |
| Loss | 0.208 |

---

## 🔍 Key Concepts Used
- **Flatten Layer** → Converts 2D image into 1D for the model
- **Dropout** → Prevents overfitting by randomly dropping neurons
- **Softmax** → Converts outputs into probabilities
- **SparseCategoricalCrossentropy** → Loss function for multi-class problems
- **Adam Optimizer** → Faster and smarter than basic SGD

---

## 🧪 Sample Prediction
Model predicted: **7**
Actual label: **7** ✅
