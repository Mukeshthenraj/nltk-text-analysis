# 📚 NLTK Text Analysis and Spelling Recommender

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![NLTK](https://img.shields.io/badge/NLTK-3.x-green)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

This project demonstrates how to use **Natural Language Toolkit (NLTK)** in Python to analyze and process large text data and build intelligent spelling recommender systems.

> **Note:** This repository was created as a personal learning project to demonstrate natural language processing techniques with NLTK. It is not affiliated with any course or institution.

---

## ✨ Features

✅ **Part 1: Text Analysis**
- Tokenizes a large collection of movie plot summaries.
- Calculates:
  - Total number of tokens
  - Number of unique tokens
  - Lexical diversity
  - Word frequencies and distributions
  - Most frequent parts of speech
  - Longest token
- Performs lemmatization to reduce words to their base forms.
- Computes statistics like percentage occurrence of specific words (e.g., *love*).

✅ **Part 2: Spelling Recommender**
- Builds three spelling recommendation engines using:
  - **Jaccard distance** on trigrams
  - **Jaccard distance** on 4-grams
  - **Edit distance** (Levenshtein distance) with transpositions
- Suggests closest-correct spellings for example misspelled words.

---

## 🗂️ Project Structure

```
.
├── text_analysis.py        # Main Python script containing all functions
├── plots.txt               # Text corpus: movie plot summaries
└── README.md               # Project description and usage instructions
```

---

## 🛠 Installation

1. **Clone this repository:**
   ```
   git clone https://github.com/<your-username>/nltk-text-analysis.git
   cd nltk-text-analysis
   ```

2. **Install dependencies:**
   ```
   pip install nltk pandas numpy
   ```

3. **Download NLTK resources:**
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('averaged_perceptron_tagger')
   nltk.download('wordnet')
   nltk.download('words')
   ```

---

## 🚀 How to Run

1️⃣ Make sure `plots.txt` is in the same directory as `text_analysis.py`.  
2️⃣ Run the script:

```bash
python text_analysis.py
```

or open the notebook version if you prefer interactive exploration.

---

## ✍️ Example Outputs

**Lexical Diversity:**
```
0.06925790712021386
```

**20 Most Frequent Tokens:**
```
(',', 19420), ('the', 18698), ('.', 16624), ...
```

**Spelling Recommendations:**
```
['corpulent', 'indecence', 'validate']
```

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## ✨ Acknowledgments

- [NLTK](https://www.nltk.org/) — Natural Language Toolkit
- CMU Movie Summary Corpus

---

⭐ **Feel free to explore, modify, or extend this project!**

