# 📰 Fake News Detector Using LSTM

## 📚 Overview

In today's digital landscape, the rapid spread of fake news has become a significant global challenge.  
This project develops a machine learning model using a Long Short-Term Memory (LSTM) neural network to classify news articles as **real** or **fake** based on their textual content.

The goal is to leverage Natural Language Processing (NLP) and deep learning techniques to build a reliable, data-driven fake news detection system.

---

## 🚀 Project Highlights

- Built an LSTM-based neural network for sequential text classification.
- Achieved **99.5% test accuracy** (0.9949) with strong precision, recall, and F1-scores.
- Applied comprehensive text cleaning (URL removal, punctuation stripping, stemming, etc.).
- Tokenized and padded text data for efficient model training.
- Implemented **EarlyStopping** to prevent overfitting.
- Evaluated the model using a confusion matrix and classification report.
- Visualized training and validation performance with accuracy and loss curves.

---

## 🛠 Technologies Used

- Python
- Jupyter Notebook
- TensorFlow / Keras
- NLTK (Natural Language Toolkit)
- Matplotlib & Seaborn
- Scikit-learn

---

## 📈 Model Performance

| Metric | Value |
|:------|:------|
| Test Accuracy | 99.5% |
| Precision (Fake News) | 100% |
| Recall (Fake News) | 99% |
| Precision (Real News) | 99% |
| Recall (Real News) | 100% |
| F1-Score | 99% |

---

## 📂 Project Structure

```plaintext
├── Fake News Detector(LSTM).ipynb    # Jupyter notebook with full project code
├── data/
    ├── Fake.csv                      # Dataset for fake news
    ├── True.csv                      # Dataset for real news
├── README.md                         # Project documentation
```

---

## ⚠️ Limitations

- The same 20% split was used as validation data for early stopping and as the final test set, so the test score is slightly optimistic. A separate hold-out set would be cleaner.
- Training was unstable in the middle: accuracy dropped to about 68% at epoch 4 before recovering.
- Many real articles start with a "(Reuters)" dateline, and the text cleaning keeps the word "reuters". The model may be learning some of the source's writing style, not only whether a story is true, so scores this high on this dataset should be read with caution.

---

## 🧐 Future Improvements

- Integrate pre-trained word embeddings (GloVe, Word2Vec).
- Implement Bidirectional LSTM architecture.
- Explore Attention Mechanisms to highlight important text features.
- Experiment with Transformer-based models like BERT.
- Add explainability with LIME or SHAP to interpret model predictions.

---

## 📜 Acknowledgments

- Datasets sourced from [Kaggle Fake and True News Dataset](https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset).
- Special thanks to the open-source machine learning and NLP communities!

---

## 📬 Contact

**Jean-Emmanuel Kouadio**  
Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/j-emmanuel-k/) or check out my other projects on [GitHub](https://github.com/jeanemmanuelk)!
