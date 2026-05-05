# 💬 Text Sentiment Classification (NLP)

Machine learning project to classify text sentiment using natural language processing techniques, supporting applications such as content moderation and customer feedback analysis.

---

## 📌 Project Overview

This project builds a sentiment classification model capable of identifying **negative vs non-negative text** from user-generated content.

Such systems are commonly used in:

- Content moderation platforms  
- Customer review analysis  
- Social media monitoring  

The goal is to transform raw text into structured features and train a model that can accurately classify sentiment.

---

## 📊 Problem

Text data is inherently unstructured and presents several challenges:

- Variability in language and writing style  
- Noise (punctuation, slang, misspellings)  
- Context-dependent meaning  

The objective is to build a model that:
- Accurately detects negative sentiment  
- Generalizes well to unseen text  
- Remains computationally efficient  

---

## 📁 Data

The dataset consists of labeled text samples, where each entry is classified as:

- Negative sentiment  
- Non-negative sentiment  

---

## ⚙️ Approach

### 1. Text Preprocessing

- Lowercasing and normalization  
- Removal of punctuation and noise  
- Tokenization of text  

---

### 2. Feature Extraction

Text was converted into numerical representations using:

- **TF-IDF (Term Frequency–Inverse Document Frequency)**  

This approach captures the importance of words relative to the dataset while maintaining computational efficiency.

---

### 3. Modeling

Trained and evaluated classification models such as:

- Logistic Regression  
- (Optional: Naive Bayes / Linear SVM if used)

These models are well-suited for high-dimensional sparse text data.

---

### 4. Evaluation

Model performance was evaluated using:

- **Accuracy**  
- **F1-score**  
- **Precision / Recall**

These metrics are particularly important for imbalanced classification tasks.

---

## 📈 Results

The best performing model on test data was the spaCy + TF-IDF + Logistic Regression model, which achieved the following scores:

- **F1-score: 0.89**  
- **Accuracy: 0.89**

The model demonstrates strong performance in identifying negative sentiment while maintaining generalization.

---

## 🔍 Key Insights

- TF-IDF representations are highly effective for baseline sentiment classification  
- Linear models perform well on high-dimensional text data  
- Certain words and phrases strongly influence sentiment predictions  
- Misclassifications often occur in cases of:
  - Sarcasm  
  - Mixed sentiment  
  - Context-dependent expressions  

---

## 🧪 Error Analysis

Examples of challenging cases include:

- Sentences with both positive and negative signals  
- Informal language or slang  
- Subtle tone differences not captured by bag-of-words approaches  

---

## 🧰 Tech Stack

- Python  
- Pandas / NumPy  
- Scikit-learn  
- NLTK / SpaCy (if used)  

---

## 🚀 How to Run

```bash
git clone https://github.com/guayasco/text-sentiment-classification.git
cd text-sentiment-classification
jupyter notebook notebook.ipynb
