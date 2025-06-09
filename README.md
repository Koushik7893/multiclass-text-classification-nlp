# 🧠 Multiclass Text Classification with Classical ML, Deep Learning, and Transformers

This repository demonstrates various approaches to solving multiclass text classification problems using traditional machine learning, deep learning (LSTMs), and modern transformer-based architectures.

---

## 📊 Datasets Used

| Dataset           | Classes | Description                                                                 |
|-------------------|---------|-----------------------------------------------------------------------------|
| **AG News**       | 4       | News headlines categorized into 4 topics: World, Sports, Business, Sci/Tech |
| **Yahoo Answers** | 10      | Community QA text, classified into 10 topics                                |
| **TREC**          | 6       | Open-domain factoid questions classified into coarse question types         |

---

## 📌 Summary Table

| Model Type       | Model               | Dataset       | Technique Highlights                                |
|------------------|---------------------|---------------|-----------------------------------------------------|
| Traditional      | Logistic Regression | AG News       | TF-IDF + One-vs-Rest, multinomial solver            |
| Deep Learning    | BiLSTM              | AG News       | GloVe + LSTM + MaxPool                              |
| Transformer Lite | DistilBERT          | Yahoo Answers | Hugging Face Trainer API, efficient fine-tuning     |
| Transformer Full | RoBERTa             | TREC          | Token-level learning + label smoothing (0.1)        |

---

## 📂 Structure

```

multiclass-text-classification-nlp/
│
├── 1\_logistic\_regression\_tfidf\_agnews.ipynb
├── 2\_bilstm\_glove\_agnews.ipynb
├── 3\_distilbert\_yahooanswers.ipynb
├── 4\_roberta\_trec\_labelsmoothing.ipynb
│
├── README.md
└── requirements.txt

````

---

## 🛠️ Key Features

- 📚 Dataset loading via Hugging Face `datasets`
- 🔤 Traditional models: TF-IDF with Logistic Regression
- 🔁 BiLSTM model with GloVe embeddings
- 🤗 Transformers via `Trainer` API (DistilBERT & RoBERTa)
- 🧪 Evaluation using accuracy, precision, recall, and F1
- ✅ Includes label smoothing (RoBERTa)

---

## 🚀 Requirements

Install required libraries using:

```bash
pip install -r requirements.txt
````

`requirements.txt`:

```
transformers
datasets
scikit-learn
numpy
pandas
matplotlib
torch
```

---

## 📈 Evaluation Metrics

Each model logs:

* Accuracy
* Precision
* Recall
* F1 Score

Evaluation is done using stratified splits or Hugging Face's `dataset["train"]` and `dataset["test"]`.

---

## 🤝 Contributing

Feel free to fork this repo and explore new datasets or models. Suggestions and pull requests are welcome!

---

## ✍️ Author

**Koushik Reddy**
🔗 [Hugging Face](https://huggingface.co/Koushim) | [LinkedIn](https://www.linkedin.com/in/koushik-reddy-k-790938257)

---

## 📌 License

This project is open source and available under the [Apache License](LICENSE).

````
