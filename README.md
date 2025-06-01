# 💬 Cyberbullying Detection and Severity Analysis using Machine Learning

This mini project presents a deep learning-based model to detect cyberbullying in social media text data and determine its severity. By integrating a Long Short-Term Memory (LSTM) neural network with a fuzzy logic system, the model offers both high accuracy and explainable severity classification.

---

## 📌 Objectives

* Automatically detect cyberbullying from social media comments.
* Use LSTM to classify text sequences as bullying or non-bullying.
* Apply fuzzy logic to determine severity levels: **Low**, **Medium**, or **High**.
* Improve accuracy, precision, recall, and F1-score compared to traditional models.

---

## 🧠 Methodology

### 🔄 Data Preprocessing

* **Dataset**: [Kaggle Cyberbullying Classification Dataset](https://www.kaggle.com/datasets/andrewmvd/cyberbullying-classification)
* **Steps**:

  * Text normalization (lowercasing, removing URLs, emojis, special characters)
  * Tokenization
  * Stop word removal
  * Lemmatization
  * Word embedding using Keras Embedding Layer

### ⚙️ Model Architecture

* **Deep Learning Model**: LSTM with 4 hidden layers (128, 64, 32, and 3 units)
* **Activation Function**: ReLU
* **Optimizer**: Adam
* **Loss Function**: Categorical Cross-Entropy
* **Output**: Binary classification (Cyberbullying vs Non-Cyberbullying)

### 🤖 Fuzzy Logic for Severity Rating

* **Input to Fuzzy System**:

  * LSTM output (toxicity score)
  * Frequency of abusive terms
* **Rules-Based System**:

  * Maps input to a severity score (0–10)
  * Classifies output as Low, Medium, or High severity
* **Advantages**:

  * Handles ambiguity better than binary logic
  * Explainable decisions through rule-based classification

---

## 📊 Dataset Details

* **Total Samples**: 47,733 tweets

  * Cyberbullying: 39,748
  * Non-Cyberbullying: 7,985

---

## 📈 Results

| Metric   | Value  |
| -------- | ------ |
| Accuracy | 82.77% |
| F1-Score | 82.43% |
| Recall   | 82.26% |

The model demonstrates strong performance and effectively identifies both cyberbullying presence and its severity.

---

## 📌 Future Work

* Extend model to support multimedia-based bullying (images, videos)
* Test model across different languages and social media platforms
* Incorporate real-time detection and alerts for moderation tools

---

## 📚 Reference

> Mohammed Hussein Obaid, Shawkat Kamal Guirguis, Saleh Mesbah Elkaffas.
> *Cyberbullying Detection and Severity Determination Model*, IEEE Access, 2023
> DOI: [10.1109/ACCESS.2023.10243022](https://ieeexplore.ieee.org/document/10243022)



