---
name: 🐛 Bug report
about: Create a report to help us improve the NLP pipeline
title: '[BUG] '
labels: 'bug'
assignees: ''

---

## 📝 Description

Briefly describe the problem. Is it a cleaning error (e.g., HTML tags still appearing), a vectorization failure, or an issue with the sentiment label encoding?

## 👣 How to Reproduce

Steps to reproduce the behavior:
1. Load the dataset `[dataset_name].csv`
2. Run the cleaning function `clean_text()`
3. Observe the output: '...' (e.g., characters like 'ñ' or 'á' are showing as corrupted symbols)
4. Error message: '...' (e.g., `UnicodeDecodeError` or `Vocabulary mismatch`)

## 🎯 Expected Behavior

A clear and concise description of what you expected to happen (e.g., the text should be entirely in lowercase, free of HTML tags, but preserving Spanish-specific characters like 'ñ').

## 🔡 Data Sample

If the bug is related to a specific review that causes a crash, please paste a sample of the text here:
```text
"Ejemplo de crítica que causa el error..."
```

## 📸 Screenshots (if applicable)

If the bug relates to terminal output or a specific plot (like a broken Confusion Matrix), please paste a screenshot or the raw text here.

## 💻 Environment

- **OS:** (e.g. Windows 11, macOS, Google Colab)
- **Python Version:** (e.g. 3.10.x)
- **NLP Libraries:** (e.g. scikit-learn 1.2, NLTK 3.8, XGBoost 1.7)

## 🔍 Additional Context

Add any other context about the problem here. If the terminal or Jupyter cell showed a specific error message (Traceback), please paste it here:
```text
[Paste your error log here]
```
