# 🧠 Binary Text Classification using Traditional Machine Learning

This project demonstrates different techniques for binary text classification using traditional machine learning models such as **Logistic Regression**, **Support Vector Machine (SVM)**, and **Naive Bayes**. It focuses on **vectorization techniques** like **TF-IDF**, **CountVectorizer**, **n-grams**, and **character-level features** to represent textual data for model training.

---

## 📌 Tasks Covered

The notebook contains a step-by-step demonstration of the following:

### 🔹 1. Loading Dataset
- Import and inspect binary-labeled text data.

### 🔹 2. Vectorization Techniques
- **TF-IDF**
- **CountVectorizer**
- **N-gram TF-IDF** (bigrams & trigrams)
- **Character-level TF-IDF**
- Visualization of fitted vectorizer (`vocabulary_`, `idf_`, etc.)

### 🔹 3. Models Implemented
| Vectorizer | Model                  | Notes                        |
|------------|------------------------|------------------------------|
| TF-IDF     | Logistic Regression     | Standard baseline            |
| CountVectorizer | Multinomial Naive Bayes | Fast, probabilistic classifier |
| TF-IDF (Bigrams) | SVM (Linear)          | Handles high-dimensionality  |
| Char-level TF-IDF | Logistic Regression     | Useful for short/spam-like texts |

---

## 🧪 Dataset

- Source: SMS Spam
- Classes: `0` (Spam), `1` (Ham)

---

## 🔧 Installation

```bash
git clone https://github.com/Koushim/text-binary-classification-classic-ml.git
cd text-binary-classification-classic-ml
pip install -r requirements.txt
````

---

## 🚀 Run on Google Colab

---

## 📂 Project Structure

```
text-binary-classification-classic-ml/
│
├── notebooks/
│   └── binary_text_classification_models.ipynb  # Main notebook
│
├── requirements.txt
└── README.md
```

---

## ✍️ Author

**Koushik Reddy**
🔗 [Hugging Face](https://huggingface.co/Koushim) | [LinkedIn](https://www.linkedin.com/in/koushik-reddy-k-790938257)

---

## 📌 License

This project is open source and available under the [Apache License](LICENSE).

````
