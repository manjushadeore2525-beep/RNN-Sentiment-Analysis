# ❤️ Sentiment Analysis using RNN, LSTM & Attention

> A deep learning project comparing **Vanilla RNN**, **LSTM**, and **Attention-based architectures** for binary sentiment classification on the IMDB Large Movie Review Dataset using TensorFlow/Keras.

<p align="center">
<img src="images/banner.png" width="100%">
</p>

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red)
![License](https://img.shields.io/badge/License-MIT-green)

---

<img width="1687" height="925" alt="image" src="https://github.com/user-attachments/assets/df7343bd-c7c0-4417-8ca1-73c89863958b" />

# 🚀 Project Highlights

- ✅ Binary Sentiment Classification
- ✅ Vanilla RNN
- ✅ Long Short-Term Memory (LSTM)
- ✅ Attention Mechanism
- ✅ Word Embeddings
- ✅ GloVe Integration
- ✅ Word2Vec Integration
- ✅ IMDB Movie Review Dataset
- ✅ Comparative Performance Analysis

---

# 📌 Project Overview

This project investigates different recurrent neural network architectures for sentiment classification.

The objective is to understand how memory mechanisms and attention improve sentiment prediction compared to traditional recurrent neural networks.

Models implemented include:

- Vanilla RNN
- LSTM
- Attention-LSTM
- Trainable Embeddings
- Static GloVe Embeddings
- Static Word2Vec Embeddings

---

# 🎯 Objectives

- Compare RNN and LSTM architectures
- Study Vanishing Gradient problems
- Evaluate pretrained embeddings
- Analyze Attention Mechanisms
- Perform Binary Sentiment Classification

---

# 📂 Dataset

**Dataset:** IMDB Large Movie Review Dataset

Dataset Statistics

- 25,000 Training Reviews
- 25,000 Testing Reviews
- Binary Sentiment Labels
- Vocabulary Size: 10,000
- Sequence Length: 150 Tokens

---

# 🔄 Data Preprocessing

The preprocessing pipeline includes:

- Lowercasing
- Punctuation Removal
- Tokenization
- Vocabulary Construction
- Integer Encoding
- Sequence Padding
- Sequence Truncation

Pipeline

```
Raw Reviews
      │
      ▼
Cleaning
      │
      ▼
Tokenization
      │
      ▼
Vocabulary Encoding
      │
      ▼
Padding
      │
      ▼
Neural Network
```

---

# 🏗️ Model Architectures

## Vanilla RNN

```
Embedding
     │
     ▼
Simple RNN
     │
     ▼
Dense
     │
     ▼
Sigmoid
```

---

## LSTM

```
Embedding
     │
     ▼
LSTM
     │
     ▼
Dense
     │
     ▼
Sigmoid
```

---

## Attention LSTM

```
Embedding
     │
     ▼
LSTM
     │
     ▼
Attention Layer
     │
     ▼
Dense
     │
     ▼
Sigmoid
```

---

# 📚 Word Embeddings

Three embedding strategies were evaluated:

### Trainable Embedding

- Learned during training
- Dataset-specific
- Adaptable

---

### GloVe

- Stanford pretrained vectors
- Global word statistics
- Frozen weights

---

### Word2Vec

- Google pretrained embeddings
- Semantic word relationships
- Frozen weights

---

# ⚙️ Training Configuration

| Parameter | Value |
|-----------|-------:|
| Vocabulary Size | 10,000 |
| Embedding Dimension | 100 |
| Hidden Units | 64 |
| Sequence Length | 150 |
| Epochs | 5 |
| Batch Size | 64 |
| Optimizer | Adam |
| Loss | Binary Cross Entropy |

---

# 📊 Results

## Embedding Comparison

| Embedding | Accuracy |
|------------|---------:|
| Trainable | 81.71% |
| GloVe | 72.20% |
| Word2Vec | 72.14% |

---

## RNN vs LSTM

| Model | Accuracy | F1 Score |
|--------|---------:|----------:|
| Vanilla RNN | 80.02% | 80.78% |
| LSTM | **84.20%** | **84.23%** |

---

## Key Observations

- LSTM outperformed Vanilla RNN.
- Trainable embeddings adapted better to the dataset.
- Attention improved long-range dependency modeling.
- LSTM significantly reduced vanishing gradient issues.

---

# 🧠 Attention Mechanism

Attention enables the model to focus on important words rather than compressing an entire review into a single hidden state.

Benefits include:

- Better context understanding
- Long-range dependency modeling
- Improved interpretability
- Higher sentiment classification accuracy

---

# 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Pandas
- Scikit-learn

---

# 📁 Repository Structure

```
RNN-Sentiment-Analysis/
│
├── data/
├── images/
│   ├── banner.png
│   ├── architecture.png
│   ├── training_curves.png
│   └── confusion_matrix.png
│
├── report/
│   └── Latex-Report.pdf
│
├── RNN-Sentiment-Analysis.ipynb
├── README.md
├── requirements.txt
├── LICENSE
├── .gitignore
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── SECURITY.md
└── .github/
    └── workflows/
        └── python.yml
```

---

# 🚀 Future Improvements

- Bidirectional LSTM
- GRU Architecture
- Transformer Encoder
- BERT Fine-tuning
- RoBERTa
- DistilBERT
- Hyperparameter Optimization
- Explainable AI (LIME & SHAP)

---

# 📚 References

- IMDB Large Movie Review Dataset
- TensorFlow Documentation
- Keras Documentation
- Word2Vec Paper
- GloVe Paper
- Bahdanau Attention
- Luong Attention

---

# 👩‍💻 Author

**Manjusha Deore**

Machine Learning Engineer | AI & Data Science

### Skills

- Natural Language Processing
- Deep Learning
- Sentiment Analysis
- RNN
- LSTM
- Attention Mechanisms
- TensorFlow
- Python

---

⭐ If you found this project useful, consider giving it a **Star**!
