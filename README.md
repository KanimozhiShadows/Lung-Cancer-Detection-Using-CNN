﻿# Lung-Cancer-Detection-Using-CNN
---

# 🧠 Lung Cancer Detection Using CNN

This project presents a deep learning-based system using **Convolutional Neural Networks (CNNs)** to detect lung cancer from medical images such as CT scans and X-rays. The aim is to aid medical professionals in early and accurate diagnosis, thereby improving patient outcomes.

---

## 📁 Dataset

We used the publicly available **Chest X-Ray Images (Pneumonia)** dataset from Kaggle:

🔗 [Chest X-Ray Dataset (Pneumonia) – Kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)

**Dataset Size**: \~2.29 GB
**Download Instructions**:

```bash
!pip install kaggle
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
!kaggle datasets download paultimothymooney/chest-xray-pneumonia
```

**Extraction:**

```python
from zipfile import ZipFile
dataset = "/content/chest-xray-pneumonia.zip"
with ZipFile(dataset, 'r') as zip:
    zip.extractall()
    print('The dataset is extracted')
```

---

## 📌 Project Objectives

* ✅ Develop an automated CNN-based classifier for lung cancer detection.
* ✅ Improve diagnosis accuracy and reduce time compared to manual analysis.
* ✅ Integrate essential preprocessing, augmentation, and evaluation techniques.
* ✅ Lay groundwork for real-world clinical integration.

---

## 🛠️ Technologies Used

* **Language**: Python
* **Frameworks & Libraries**:

  * TensorFlow / Keras
  * NumPy, Pandas
  * OpenCV
  * Matplotlib, Seaborn
  * Scikit-learn

---

## ⚙️ Model Architecture

The CNN model includes:

* Multiple convolutional and pooling layers
* ReLU activation
* Fully connected layers
* Softmax output layer for classification

Training was done using labeled grayscale CT scan images.

---

## 📊 Results

* **Accuracy**: 95.6%
* **Precision**: 94.8%
* **Recall (Sensitivity)**: 96.2%
* **Validation Accuracy**: 94.2%
* **Confusion Matrix**:

  * True Positives: 250
  * True Negatives: 230
  * False Positives: 14
  * False Negatives: 10

---

## 🧪 Modules Description

| Module                   | Description                                      |
| ------------------------ | ------------------------------------------------ |
| `NumPy`                  | Fast array manipulation and numerical operations |
| `Pandas`                 | Data preprocessing and tabular analysis          |
| `Matplotlib` / `Seaborn` | Data visualization                               |
| `OpenCV`                 | Image manipulation and processing                |
| `Keras`                  | Building and training deep learning models       |

---

## 💻 System Requirements

### Software:

* Python
* Google Colab or Jupyter Notebook

### Hardware:

* Recommended: 16GB RAM, NVIDIA RTX 2070 GPU or better

---

## 📌 How to Run

1. Clone the repository or open the Jupyter notebook.
2. Download and extract the dataset using Kaggle API.
3. Run the cells sequentially in `Lung_Cancer_Detection.ipynb`.

---

## 📄 Report

Detailed project documentation, analysis, methodology, and results can be found in:

📄 `Lung Cancer Detection Report.pdf`

---


## 📚 References

1. [GeeksforGeeks: CNN Lung Cancer Detection](https://www.geeksforgeeks.org/lung-cancer-detection-using-convolutional-neural-network-cnn/)
2. [Kaggle Dataset - Chest X-ray (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
3. [Nature.com Article](https://www.nature.com/articles/s41598-023-29656-z)
4. [ScienceDirect Article](https://www.sciencedirect.com/science/article/pii/S2665917422002227)


