
# 🧠 Sentiment Analysis – Twitter US Airline Dataset  
### 💼 Internship Task: Sentiment Analysis | Domain: Data Analysis

---

## 📝 Project Overview

This project applies Natural Language Processing (NLP) techniques to analyze airline-related tweets and classify them as **positive**, **neutral**, or **negative**. It helps evaluate customer sentiment toward different airlines using real-world Twitter data.

---

## 🎯 Key Objectives
- ✅ Clean and preprocess tweet text for NLP
- ✅ Visualize sentiment trends and keyword usage
- ✅ Build and compare machine learning models for sentiment classification

---

## 📌 Main Steps Executed

### 🔹 Data Cleaning & Preprocessing
- Removed URLs, mentions, punctuation, and stopwords
- Tokenized and lemmatized tweets
- Created a cleaned `text` column for analysis

### 🔹 Exploratory Analysis
- Visualized overall sentiment distribution
- Compared sentiment across airlines
- Generated WordClouds for each sentiment class

### 🔹 Machine Learning Models
| Model | Accuracy |
|-------|----------|
| ✅ Logistic Regression | **80%** |
| SVM (LinearSVC)        | 79% |
| Random Forest          | 77% |
| Naive Bayes            | 73% |

- Logistic Regression performed best overall and was selected as the final model.

---

## 🧪 Evaluation Highlights
- Negative sentiment is most frequent (~62%)
- Neutral tweets are hardest to classify due to their ambiguity
- Class imbalance and informal language in tweets slightly limit model accuracy

---

## 🛠️ Tools & Libraries Used
**Python**, **Jupyter Notebook**, **Pandas**, **NLTK**, **Scikit-learn**, **Matplotlib**, **Seaborn**, **WordCloud**

---

## 📌 Final Notes
> The project includes clear markdown documentation, visual insights, and model comparisons to support transparency and decision-making. Results can be further improved with advanced models like BERT or RNNs in future work.
