# 📘 Sentiment Analysis on Amazon Review Dataset

This project performs sentiment analysis on Amazon product reviews using natural language processing and machine learning. It includes customized text cleaning, feature extraction, and classification to predict review sentiment (positive or negative).

---

## 🧾 Dataset

- Source: [Kaggle - Amazon Reviews](https://www.kaggle.com/datasets/kritanjalijain/amazon-reviews)
- Key columns used:
  - `Title`: Short review title
  - `Review`: Full review text
  - `Polarity`: Target sentiment label

---

## 🔄 Preprocessing Steps

1. Combine `Title` + `Review` into a `Full_review` column
2. Convert text to lowercase
3. Remove HTML tags, URLs, and special characters
4. Remove stopwords, but **retain negations** like `not`, `no`, and `n't`
5. Apply lemmatization to normalize words

---

## 🤖 Model Pipeline

- **Vectorization**: TF-IDF
- **Classifier**: Logistic Regression / Naive Bayes
- **Split**: 80-20 train-test with stratification

---

## 📊 Example Output

| Raw Review | Cleaned Review |
|------------|----------------|
| "This is not a good product at all!" | `not good product` |

---

## 🛠️ Tech Stack

- Python 3
- pandas, numpy
- nltk
- scikit-learn

---

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/amazon-sentiment-analysis.git
   cd amazon-sentiment-analysis
2. Install required libraries:

 ```bash
pip install -r requirements.txt
 ```
3. Run the notebook or script:

 ```bash

jupyter notebook sentiment_analysis.ipynb
 ```
