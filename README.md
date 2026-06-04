# 📧 Spam Email Detector

> A Machine Learning model that automatically detects whether an email is **spam or normal** using Natural Language Processing and Naive Bayes — built with Python and Scikit-Learn.

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?logo=scikit-learn&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-Text_Classification-purple)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![ML](https://img.shields.io/badge/ML-Naive_Bayes-9cf)

---

## 📌 About this project

Spam emails are one of the biggest problems in digital communication. This project builds an intelligent system that reads an email and automatically decides if it is spam or a normal email — using **Natural Language Processing (NLP)** and a **Naive Bayes classifier**.

I built this to learn how machines can understand and classify human language — one of the most exciting areas of Artificial Intelligence.

---

## 🎯 Problem Statement

```
Given:
  → The text content of an email

Predict:
  → Is this email SPAM or NORMAL?
```

---

## 🗂️ Dataset

I created a balanced dataset of 30 emails — 15 spam and 15 normal.

| Label | Count | Examples |
|-------|-------|---------|
| Spam (1) | 15 | Prize offers, fake warnings, money schemes |
| Normal (0) | 15 | Meeting requests, project updates, greetings |

---

## 🔄 Project Workflow

```
Create Email Dataset
        ↓
Convert Text to Numbers (CountVectorizer)
        ↓
Visualize Spam vs Normal distribution
        ↓
Split Train and Test (80/20)
        ↓
Train Naive Bayes Classifier
        ↓
Evaluate with Accuracy and Confusion Matrix
        ↓
Test with Custom Email Input
```

---

## 📊 Model Results

| Metric | Result |
|--------|--------|
| Algorithm | Multinomial Naive Bayes |
| Accuracy | ~100% on test set |
| Train/Test Split | 80% / 20% |
| Text Processing | CountVectorizer (Bag of Words) |

---

## 🖼️ Visualizations included

- 📊 Spam vs Normal bar chart
- 🥧 Spam ratio pie chart
- 🔥 Confusion Matrix heatmap

---

## 💡 Sample predictions

```python
predict_email("Congratulations! You won a free iPhone. Click now!")
# Spam Probability : 98.7%
# Result : 🚨 SPAM

predict_email("Hi, please review the attached report before Friday.")
# Spam Probability : 1.2%
# Result : ✅ NORMAL

predict_email("Make money fast! Earn $500 daily working from home!")
# Spam Probability : 96.4%
# Result : 🚨 SPAM
```

---

## 🧠 How it works

```
1. Email text comes in
         ↓
2. CountVectorizer converts words into numbers
   "free prize click" → [0, 1, 0, 1, 1, 0 ...]
         ↓
3. Naive Bayes calculates probability
   P(spam | words) vs P(normal | words)
         ↓
4. Higher probability wins → Final decision
```

---

## 🛠️ Tech stack

| Tool | Purpose |
|------|---------|
| Python | Programming language |
| Pandas | Data handling |
| NumPy | Numerical computation |
| Matplotlib | Charts |
| Seaborn | Heatmap visualization |
| Scikit-Learn | NLP and ML model |
| CountVectorizer | Convert text to numbers |
| Jupyter Notebook | Development environment |

---

## 🚀 How to run

**On Google Colab — no installation needed**
1. Open the `.ipynb` file in this repository
2. Click **Open in Colab**
3. Click **Runtime → Run all**

**On local machine**
```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
jupyter notebook Spam_Email_Detector.ipynb
```

---

## 📁 Repository structure

```
Spam-Email-Detector/
├── Spam_Email_Detector.ipynb   # main notebook
└── README.md                   # project documentation
```

---

## 🔮 What I plan to add next

- [ ] Use a real dataset — SMS Spam Collection from Kaggle (5000+ emails)
- [ ] Try TF-IDF vectorizer instead of CountVectorizer
- [ ] Compare with Support Vector Machine (SVM) model
- [ ] Add a simple web interface where user types email and gets result
- [ ] Deploy online using Streamlit

---

## 🧠 What I learned

This project introduced me to **Natural Language Processing** — teaching a machine to understand text. The most interesting part was learning how CountVectorizer converts words into numbers so the ML model can process them. I also learned why Naive Bayes works so well for text classification — it is fast, simple and surprisingly accurate even with a small dataset.

---

## 🔗 Related repositories

- 📂 [ML-Practice](https://github.com/rayhan-uddin9/ML-Practice) — ML learning and practice notebooks
- 📂 [Student-Performance-Predictor](https://github.com/rayhan-uddin9/Student-Performance-Predictor) — Logistic Regression project
- 📂 [House-Price-Prediction](https://github.com/rayhan-uddin9/House-Price-Prediction) — Linear Regression project
- 📂 [Python-Documentation](https://github.com/rayhan-uddin9/Python-Documentation) — 30-class Python training course

---

> 🎓 **Rayhan Uddin** · Computer Science Student · Bangladesh
>
> *"Teaching a machine to read and understand human language is one of the most fascinating challenges in Computer Science."*
