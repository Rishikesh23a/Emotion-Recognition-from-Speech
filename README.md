# 🎤 Emotion Recognition from Speech

This project demonstrates a deep learning model to recognize emotions in spoken audio using Convolutional Neural Networks (CNNs). The implementation is built in **Python** using **Google Colab**, making it easy to reproduce and experiment.

---

## 📘 Overview

The model uses the **RAVDESS** dataset, a popular corpus of emotional speech, to classify audio recordings into eight emotions:
- Neutral
- Calm
- Happy
- Sad
- Angry
- Fearful
- Disgust
- Surprised

Features are extracted as **MFCCs** (Mel Frequency Cepstral Coefficients) and fed into a CNN for classification.

---

## 🚀 Getting Started

You can run the project directly in **Google Colab** without any setup.

### 🔗 Open in Colab
[![Open In Colab](https://colab.research.google.com/drive/1bYVjWnFHR-eaztAQdlaNx6C9lV7FVB1k?usp=sharing)

🛠️ Project Workflow

1.Download & Extract Dataset.

- Automatically downloads RAVDESS audio data.

Feature Extraction

Computes 40 MFCCs per audio file.

Pads sequences to a fixed length for input consistency.

Label Encoding

Encodes emotion labels to numeric classes.

Data Splitting

Train/Test split (80/20).

Model Building

CNN with:

2 convolutional blocks

Dropout for regularization

Dense classifier

Training

Trains for up to 30 epochs with early stopping and model checkpointing.

Evaluation

Accuracy and loss plots

Confusion matrix

Per-class precision, recall, F1-score
