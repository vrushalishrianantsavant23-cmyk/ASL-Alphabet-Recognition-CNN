# 🤟 ASL Alphabet Recognition using CNN

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZUIu_8nWBdXK7oeE2xGrWUsuQISRtstJ?usp=sharing)
![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-CNN-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📌 Project Description

This project focuses on recognizing static hand gestures from the **American Sign Language (ASL) alphabet** using a **Convolutional Neural Network (CNN)**.

ASL is widely used within the deaf community for communication. Automating ASL recognition can help **bridge communication gaps** and build more **accessible technology** for everyone.

> **Course-Based Deep Learning Project**
> **Submitted by:** Vrushali Savant
> **Enrollment Number:** 23STUCHH010296
> **Under the Guidance of:** Suresh Sir

---

## 🎯 Problem Statement

> Develop a deep learning model capable of recognizing hand signs from the ASL alphabet. The model classifies an input image into one of the **24 ASL letters (A–Y, excluding J and Z)**, which are represented as static gestures.

CNNs are well suited for this task because they extract spatial features from images, enabling accurate gesture classification.

---

## 📂 Dataset

| Detail | Info |
|--------|------|
| **Name** | Sign Language MNIST |
| **Source** | [Kaggle Dataset](https://www.kaggle.com/datasets/datamunge/sign-language-mnist) |
| **Files** | `sign_mnist_train.csv`, `sign_mnist_test.csv` |
| **Image Size** | 28×28 pixels (Grayscale) |
| **Classes** | 24 (A–Y, excluding J & Z) |

---

## 🧠 Model Architecture

```
Input (28×28×1)
    ↓
Conv2D (32 filters, 3×3, ReLU)
    ↓
MaxPooling2D (2×2)
    ↓
Conv2D (64 filters, 3×3, ReLU)
    ↓
MaxPooling2D (2×2)
    ↓
Flatten
    ↓
Dense (128 units, ReLU)
    ↓
Dense (24 units, Softmax)  ← Output
```

- **Optimizer:** Adam
- **Loss Function:** Sparse Categorical Crossentropy
- **Epochs:** 10
- **Batch Size:** 64

---

## 📊 Results

The model produces:
- ✅ **Training & Validation Accuracy Curves**
- ✅ **Training & Validation Loss Curves**
- ✅ **Visual predictions on test images (True vs Predicted labels)**

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Programming Language |
| TensorFlow / Keras | Model Building & Training |
| NumPy & Pandas | Data Processing |
| Matplotlib | Visualization |
| Scikit-learn | Label Encoding |
| Google Colab | Development Environment |

---

## 🚀 How to Run

### Option 1 — Run on Google Colab (Recommended)
1. Click the **Open in Colab** badge above
2. Upload `sign_mnist_train.csv` and `sign_mnist_test.csv` to Colab
3. Run all cells in order

### Option 2 — Run Locally
```bash
# 1. Clone this repository
git clone https://github.com/YOUR_USERNAME/ASL-Alphabet-Recognition-CNN.git
cd ASL-Alphabet-Recognition-CNN

# 2. Install dependencies
pip install -r requirements.txt

# 3. Download the dataset from Kaggle and place CSVs in the project folder

# 4. Run the script
python deep_learning.py
```

---

## 📦 Requirements

```
tensorflow
numpy
pandas
matplotlib
scikit-learn
kaggle
```

> Install all at once: `pip install -r requirements.txt`

---

## 📁 Project Structure

```
ASL-Alphabet-Recognition-CNN/
│
├── DEEP_LEARNING.ipynb       # Main Colab Notebook
├── deep_learning.py          # Python script version
├── requirements.txt          # Dependencies
└── README.md                 # Project documentation
```

---

## 🙌 Acknowledgements

- Dataset by [Kaggle - Sign Language MNIST](https://www.kaggle.com/datasets/datamunge/sign-language-mnist)
- TensorFlow/Keras documentation
- Deep Learning course guidance by **Suresh Sir**

---

## 📃 License

This project is for **educational purposes** as part of a Deep Learning course.

---

*Made with ❤️ by Vrushali Savant*
