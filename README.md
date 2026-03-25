# B23CM1011-A2
# 🚀 NLU Assignment: Word Embeddings & Name Generation

<p align="center">
  <b>Natural Language Understanding Project</b><br>
  Word2Vec + Character-Level Neural Networks (from scratch using NumPy)
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue">
  <img src="https://img.shields.io/badge/Numpy-✔️-orange">
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen">
</p>

---

# 📌 Overview

This project implements two major NLP tasks:

### 🔹 Problem 1: Word Embeddings

* Train **Word2Vec models (CBOW & Skip-gram)**
* Use real-world data scraped from IIT Jodhpur
* Perform semantic analysis & visualization

### 🔹 Problem 2: Name Generation

* Generate Indian names using:

  * Vanilla RNN
  * BLSTM
  * Attention-based RNN
* Evaluate using novelty & diversity metrics

---

# 📂 Project Structure

```bash
Assignment/
│
├── Problem1/
│   ├── scraper.py
│   ├── build_corpus.py
│   ├── main_word2vec.py
│   ├── data/raw/
│   ├── iitj_corpus_raw.txt
│   ├── outputs/
│
├── Problem2/
│   ├── problem2_name_gen.py
│   ├── TrainingNames.txt
│   ├── outputs/
│
└── README.md
```

---

# ⚙️ Installation

```bash
pip install numpy matplotlib requests beautifulsoup4 lxml pdfplumber
```

---

# 🧠 Problem 1: Word2Vec on IIT Jodhpur Data

## 🔍 Step 1: Scraping Data

```bash
python scraper.py
```

✔ Collects data from:

* Departments
* Academics
* Research
* Faculty
* Announcements

---

## 🧾 Step 2: Build Corpus

```bash
python build_corpus.py
```

✔ Creates:

```bash
iitj_corpus_raw.txt
```

---

## 🤖 Step 3: Train Word2Vec

```bash
python main_word2vec.py
```

---

## 📊 Outputs

* 📄 Clean corpus → `iitj_corpus_clean.txt`
* 📊 Word frequency plot → `task1_wordcloud.png`
* 📈 Embedding visualization → `embedding.png`

---

## 🔬 Features

* CBOW & Skip-gram (from scratch)
* Hyperparameter tuning
* Cosine similarity
* Word analogies
* PCA visualization

---

# 🤖 Problem 2: Character-Level Name Generation

## ▶️ Run the Model

```bash
python problem2_name_gen.py
```

---

## ⚙️ Models Implemented

* 🔹 Vanilla RNN
* 🔹 Bidirectional LSTM (BLSTM)
* 🔹 Attention-based RNN

---

## 📊 Outputs

```bash
TrainingNames.txt
generated_names_VanillaRNN.txt
generated_names_BLSTM.txt
generated_names_AttentionRNN.txt
p2_training_curves.png
```

---

## 📈 Evaluation Metrics

| Metric    | Description                     |
| --------- | ------------------------------- |
| Novelty   | % of names not in training data |
| Diversity | % of unique generated names     |

---

## 📊 Sample Results

| Model
