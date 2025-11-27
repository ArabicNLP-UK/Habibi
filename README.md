# Habibi: A Multi-Dialect, Multi-National Arabic Song Lyrics Corpus

**Habibi** is the first large-scale open corpus of Arabic song lyrics, comprising more than **30,000 songs** performed by artists from **18 Arab countries**. The collection represents **six major Arabic dialect groups**, segmented into over **520,000 verses** and containing more than **3.5 million words**. 

The corpus was designed to support computational research in **Arabic dialect identification**, **country-of-origin classification**, **authorship analysis**, and wider studies in Arabic language variation within contemporary music.

---

## 🌍 Corpus Overview

The Habibi corpus brings together lyrics from across the Arab world, reflecting the linguistic and cultural diversity of modern Arabic music. Each song includes:

- **Singer name**
- **Song title**
- **Country of origin**
- **Dialect category**  
  (Egyptian, Gulf, Levantine, Iraqi, Sudanese, Maghrebi)
- **Writer and composer** (where available)
- **Lyrics segmented into verses**

All lyrics were collected using a Web-as-Corpus approach and manually curated to maintain a clean, noise-free dataset free of emojis, hashtags, and social-media artefacts.

### Key Statistics

| Item | Count |
|------|-------|
| Songs | 30,072 |
| Verses (sentences) | 527,870 |
| Words | 3.57 million |
| Singers | 1,765 |
| Writers | 3,789 |
| Composers | 2,463 |
| Countries | 18 |
| Dialects | 6 |

---

## 🗂 Dialects and Geographic Coverage

Songs are categorised into six dialect groups widely recognised across modern Arabic music:

- **Egyptian**
- **Gulf**
- **Levantine**
- **Iraqi**
- **Sudanese**
- **Maghrebi**

Although singers often perform in dialects other than their own, the corpus assigns dialect based on the singer’s country of origin, following conventions used by major Arabic music platforms (Anghami, Spotify, Deezer).

---

## 📁 File Formats

The corpus is distributed in several machine-readable formats to support a range of NLP tasks:

### **1. CSV (primary format)**  
Contains all metadata fields and verse-level text in UTF-8.

### **2. Annotated TXT**  
Each song is provided as a structured, UTF-8 annotated document with lightweight XML-style tags identifying metadata and verse boundaries.

### **3. JSON & XML**  
Converted directly from the CSV, preserving all metadata and text segmentation.

---

## 🔧 Recommended Use-Cases

Researchers may use Habibi to explore:

- Arabic **dialect identification** (sentence- or song-level)
- **Country-of-origin classification**
- **Authorship attribution** (singers, songwriters)
- **Linguistic variation** in modern Arabic music
- **Embeddings training** using domain-specific lyrics
- **Sociolinguistic analysis** of themes, vocabulary, and regional patterns

The dataset has demonstrated strong performance across classical and deep-learning models, including CNN, LSTM, CLSTM, BiGRU, and BiLSTM architectures.

---

## 📊 Benchmarks

Extensive experiments were conducted on:

- **Binary dialect classification**  
- **Multi-class dialect classification (3–6 classes)**
- **Binary country-of-origin classification**
- **Multi-class country classification (3–18 classes)**

Models tested include:

- Naïve Bayes, Logistic Regression, SVM  
- CNN, LSTM, BiLSTM, CLSTM, BiGRU  
- FastText Arabic word embeddings  
- In-house **Habibi CBOW embeddings** (300-dimensional)

**The word-level CNN model** achieved the strongest deep-learning results, while **Naïve Bayes** consistently performed best among classical models on multi-class tasks.

---

## 📦 Download

All formats (CSV, TXT, JSON, XML) as well as **Habibi’s in-house word embeddings** are available for free research use.

Original repository:  
http://ucrel-web.lancaster.ac.uk/habibi/

---

## 📝 Citation

If you use the Habibi corpus, please cite:

**El-Haj, M. (2020).**  
*Habibi – a multi-dialect multi-national Arabic song lyrics corpus.*  
In **Proceedings of the Twelfth Language Resources and Evaluation Conference (LREC 2020)**, pp. 1318–1326.  
URL: https://www.lancaster.ac.uk/staff/elhaj/docs/habibi.pdf

### BibTeX
```bibtex
@inproceedings{elhaj2020habibi,
  title={Habibi--a multi dialect multi national Arabic song lyrics corpus},
  author={El-Haj, Mahmoud},
  booktitle={Proceedings of the Twelfth Language Resources and Evaluation Conference},
  pages={1318--1326},
  year={2020}
}
