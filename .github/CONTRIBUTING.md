# Contributing to Movie Review Sentiment Analysis

Thank you for your interest in improving our NLP pipeline! This project is a space to experiment with text processing, linguistics, and machine learning. We welcome any contribution that helps us better understand the nuances of the Spanish language and improves our sentiment classification.

## How to Contribute

1. **Fork** the repository.
2. Create your branch: `git checkout -b feature/nlp-improvement`.
3. Make your changes (e.g., a new cleaning regex or a different vectorizer).
4. Commit your changes: `git commit -m "Add Lemmatization to the preprocessing pipeline"`.
5. Push your branch: `git push origin feature/nlp-improvement`.
6. Open a **Pull Request**.

## 💡 Ideas for Contribution

- **Advanced Text Normalization:** Implement **Lemmatization** or **Stemming** specifically for Spanish to reduce the vocabulary size and group related words.
- **Word Embeddings:** Move beyond TF-IDF by implementing **Word2Vec**, **FastText**, or **GloVe** to capture semantic relationships between words.
- **Transformer Models:** Experiment with **BERT** (specifically *BETO*, the Spanish BERT) to see if context-aware embeddings improve the Kaggle score.
- **N-grams Analysis:** Experiment with bigrams or trigrams in the `TfidfVectorizer` to capture phrases like "no es bueno" instead of just individual words.
- **Feature Importance:** Create visualizations to show which words are the strongest predictors for "Positive" vs "Negative" sentiments.
- **Handling Sarcasm:** Research and implement techniques to detect sarcasm or complex negations in movie reviews.



## 🧪 Development Guidelines

- **Spanish Language Focus:** All cleaning and tokenization logic must be optimized for Spanish (handling tildes, "ñ", and specific stop-words).
- **Metric-Driven:** Any change to the model or vectorizer should be accompanied by a comparison of **F1 Score** and **Accuracy**.
- **Vectorization Consistency:** Ensure that any change in the training pipeline is perfectly replicated in the prediction pipeline for the Kaggle test set.
- **Efficiency:** Since the dataset has 50k reviews, try to keep the preprocessing functions vectorized (using Pandas/NumPy) rather than using slow Python loops.
- **Clean Notebooks:** Please restart the kernel and run all cells before submitting to ensure the notebook is reproducible.

## 🏗️ NLP Pipeline Flow

1. **Filtering:** Language detection and noise removal.
2. **Cleaning:** Stripping HTML, punctuation, and numbers.
3. **Vectorization:** TF-IDF or Embedding generation.
4. **Classification:** Training and cross-validation.

Thank you for helping us push the boundaries of sentiment analysis! 🚀🔡
