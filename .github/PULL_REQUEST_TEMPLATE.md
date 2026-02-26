# 🚀 Pull Request - NLP Model Update

## 📝 Description

Briefly describe the changes in this PR:
- What part of the NLP pipeline was modified? (Cleaning, Tokenization, Vectorization, Modeling).
- Did you modify the `TfidfVectorizer` parameters or the Stopwords list?

### 📊 Metric Impact
*Please report the performance changes (compare with Naive Bayes baseline if applicable):*
- **F1 Score:** (Increased/Decreased/Maintained)
- **Kaggle Score:** (If a submission was made)
- **Training Time:** (Did the vectorization become significantly slower?)

---

## 🏗️ Type of Change
Please check the relevant option:
- [ ] 🧹 Text Cleaning update (Regex, HTML stripping, etc.)
- [ ] 🔡 Vectorization change (TF-IDF, CountVectorizer, Word2Vec)
- [ ] 🧪 New Model implementation
- [ ] 📚 Stopwords / Dictionary update
- [ ] 📝 Documentation / Notebook update

---

## ✅ NLP Checklist

- [ ] **Preprocessing Consistency:** Verified that the same cleaning steps are applied to both Training and Test sets.
- [ ] **Vocabulary Size:** Checked if the number of features (words) in TF-IDF is within a manageable range.
- [ ] **Language Check:** Confirmed the cleaning logic is still optimized for the Spanish language.
- [ ] **Reproducibility:** Used a fixed `random_state` for model splitting and training.
- [ ] **Notebook Hygiene:** The Jupyter Notebook has been cleared of outputs to keep the file size low.

---

## 📸 Visualizations (Optional)
*Attach any new Word Clouds, Top-N Word frequency bars, or Confusion Matrices.*



---

Thanks for your contribution to **Críticas de Películas**! 🎬
