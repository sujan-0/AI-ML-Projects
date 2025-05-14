# Hotel Review Sentiment Rating using Deep Learning

This repository contains the implementation of various deep learning models to predict hotel review ratings based on the sentiment of the text reviews. The project also features a Streamlit-based web application for real-time review rating prediction.

---

## 📊 Overview

This assignment explores three different neural network architectures:

* **Model 1:** Simple RNN
* **Model 2:** LSTM
* **Model 3:** LSTM with Word2Vec embeddings

The models are trained and evaluated on a dataset of hotel reviews, aiming to classify review ratings on a scale of 1 to 5.

---

## 🚀 Key Features

* Text preprocessing pipeline (cleaning, tokenization, lemmatization)
* Visual representation of review content using WordCloud
* Tokenization and sequence padding for deep learning
* Implementation of Word2Vec to enhance embedding layer
* Streamlit web app for real-time rating prediction

---

## 📄 Dataset

* **File**: `Hotel_Reviews.csv`
* **Columns**: `Review`, `Rating`

---

## 💡 Technologies Used

* Python
* TensorFlow & Keras
* NLTK
* Gensim (Word2Vec)
* Matplotlib & WordCloud
* Scikit-learn
* Streamlit

---

## 🔄 Installation & Usage

```bash
# Clone the repo
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name

# Install dependencies
pip install -r requirements.txt

# Run the Streamlit app
streamlit run app.py
```

---

## 🔢 Models & Evaluation

Each model was trained for 10 epochs with early stopping enabled. Accuracy hovered around 42% due to class imbalance:

* Model 1 (Simple RNN)
* Model 2 (LSTM)
* Model 3 (LSTM + Word2Vec) – Best performer 

Evaluation metrics include:

* Accuracy
* Confusion Matrix
* Classification Report

---

## 📅 Results Summary

| Model           | Accuracy |
| --------------- | -------- |
| Simple RNN      | ≈ 51%    |
| LSTM            | ≈ 54%    |
| LSTM + Word2Vec | ≈ 60%    |

---

## 📖 GUI for Real-Time Prediction

A simple Streamlit app allows users to enter a hotel review and receive a predicted rating (1-5).

---

## 🚜 Future Work

* Improve data balancing
* Use transformer-based models like BERT
* Deploy via Docker or cloud service

---

Feel free to explore, fork, and contribute to the project!
