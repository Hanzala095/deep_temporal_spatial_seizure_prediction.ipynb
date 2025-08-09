# Deep Temporal-Spatial Attention Network for Seizure Prediction

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-1.10%2B-red)](https://pytorch.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📌 Overview
This project implements a **Deep Temporal-Spatial Attention Network** for EEG-based seizure prediction, developed as part of the **ITSOLERA Internship (Machine Learning Track)**.  
It uses the **CHB-MIT Scalp EEG Database** to preprocess EEG signals, segment them into time windows, and predict seizures using deep learning.

## 🧠 Key Features
- EEG Preprocessing: bandpass filter (0.5–40 Hz) and notch filter (49–51 Hz)
- Window segmentation and seizure/non-seizure labeling
- Temporal and Spatial multi-head attention layers
- Training, validation, and evaluation pipeline
- Metrics: Accuracy, AUC, and Confusion Matrix

## 📂 Dataset
The dataset used is the **CHB-MIT Scalp EEG Database**, available at PhysioNet:  
🔗 [https://physionet.org/content/chbmit/1.0.0/](https://physionet.org/content/chbmit/1.0.0/)

**Structure after download**:
data/
└── chbmit/
├── chb01_01.edf
├── chb01_02.edf
└── 
## ⚙️ Installation
Clone this repository and install dependencies:
git clone https://github.com/<your-username>/deep-temporal-spatial-seizure-prediction.git
cd deep-temporal-spatial-seizure-prediction
pip install -r requirements.txt
🚀 Usage
Run on Google Colab:

Upload the .ipynb notebook to Google Colab.

Mount or upload the data/chbmit/ folder containing the CHB-MIT EEG files.

Run all cells in order.

🏗 Model Architecture
The Deep Temporal-Spatial Attention Network is composed of:

Temporal Attention Module – captures time-dependent EEG patterns

Spatial Attention Module – models inter-channel relationships

Fully Connected Layers – for classification

📊 Results
Metric	Value
Accuracy	~94%
AUC	0.71
Classes	Seizure / Non-Seizure

Example Confusion Matrix:
[[68  0]
 [ 4  0]]
 
📜 License
This project is licensed under the MIT License – see the LICENSE file for details.

🤝 Acknowledgements
PhysioNet CHB-MIT Dataset

MNE-Python for EEG processing

PyTorch for deep learning implementation

ITSOLERA Pvt Ltd – Internship Project
