# 🎬 Movie Review Sentiment Analysis (NLP)

A Natural Language Processing (NLP) project focused on classifying movie reviews as positive or negative. Developed as a competitive entry for **FIUBA**, this repository explores the full text-processing pipeline, from language filtering and tokenization to advanced ensemble classification.



# 📸 Overview
The goal was to predict sentiment on a dataset of 50,000 reviews. The challenge required deep text cleaning and vectorization strategies to handle the nuances of the Spanish language, ultimately testing multiple architectures to find the best balance between complexity and performance.

# 📍 Table of Contents
- [📝 Description](#-description)
  - [🧹 Text Preprocessing](#-text-preprocessing)
  - [🔍 Models Explored](#-models-explored)
- [📊 Performance Metrics](#-performance-metrics)
- [📈 Key Insights](#-key-insights)
- [🛠️ Technologies](#️-technologies)
- [👥 Team](#-team)
- [📄 License](#-license)

---

# 📝 Description
This project focuses on **Sentiment Analysis** in Spanish. The main challenge was the high dimensionality of text data and the presence of noise (multi-language reviews and special characters).

## 🧹 Text Preprocessing
Since the quality of an NLP model depends heavily on the input data, we implemented a rigorous cleaning pipeline:
- **Language Filtering:** Detected and removed non-Spanish reviews, reducing the set to 48,183 high-quality samples.
- **Text Normalization:** Removal of special characters, HTML tags, and numerical noise.
- **Vectorization (TF-IDF):** Utilized `TfidfVectorizer` to transform text into numerical features, applying Spanish stop-word removal to focus on sentiment-carrying terms.



## 🔍 Models Explored
We benchmarked several algorithms to compare their effectiveness in high-dimensional sparse data:
- **Naive Bayes:** The baseline and overall winner for this specific task.
- **Tree-based Ensembles:** Random Forest and **XGBoost**.
- **Deep Learning:** Neural Networks (MLP) for capturing non-linear patterns.
- **Meta-Learning:** A **Stacking** architecture to combine the strengths of individual classifiers.

---

# 📊 Performance Metrics

| Model | F1 Score | Precision | Recall | Accuracy | Kaggle Score |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Naive Bayes (Best)** | **0.8691** | 0.8591 | 0.8793 | 0.8674 | **0.7503** |
| Random Forest | 0.8533 | 0.8357 | 0.8716 | 0.8500 | 0.7228 |
| XGBoost | 0.8602 | 0.8513 | 0.8693 | 0.8586 | 0.7047 |
| Neural Network | **0.8767** | **0.8767** | 0.8767 | **0.8767** | 0.7447 |
| Stacking | 0.8676 | 0.8453 | **0.8911** | 0.8629 | 0.7462 |

---

# 📈 Key Insights
- **Simplicity Wins:** Despite the complexity of Neural Networks and Stacking, **Naive Bayes** provided the best generalization on the Kaggle hidden test set. This is often true in NLP with TF-IDF due to the independence assumption working well with word frequencies.
- **Data Cleaning Impact:** Removing English reviews and cleaning specific Spanish characters was the single most effective step in improving the F1 Score.
- **Feature Sparsity:** Text data creates very sparse matrices; models like Naive Bayes handle this sparsity more efficiently than dense models without extensive tuning.

---

# 🛠️ Technologies
- **Language:** Python 3.x
- **NLP & ML:** Scikit-learn, XGBoost, NLTK
- **Data Handling:** Pandas, NumPy
- **Visualizations:** Matplotlib, Seaborn

---

# 👥 Team
| Member | GitHub |
| :--- | :--- |
| **Sebastián Brizuela** | [@SebaB29](https://github.com/SebaB29) |
| **Lucía Agha Zadeh Dehdeh** | [@Lucia-azd](https://github.com/Lucia-azd) |
| **Juan Sebastián Del Río** | [@S2JuanS2](https://github.com/S2JuanS2) |

---

# 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
