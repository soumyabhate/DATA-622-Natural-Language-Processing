# 📚 DATA 622 — Natural Language Processing

**Author:** Soumya Bhate  
**Instructor:** Prof. Tony Diana

---

## 1) Course Description
These are my Assignments for the **Data 622 — Natural Language Processing** course in my **3rd semester at UMBC**, taught by **Prof. Tony Diana**.

---

## 2) Assignments Include

**Assignment 1 — Web Scraping Basics**  
Requests + BeautifulSoup to fetch pages, extract visible text/headings/links, and save snippets.

**Assignment 2 — Text Cleaning & Normalization**  
Lowercasing, HTML/punctuation stripping, stopword removal, and stemming vs. lemmatization.

**Assignment 3 — Similarity & Embeddings**  
Compare TF-IDF cosine with sentence embeddings; measure sentence/document similarity for retrieval.

**Assignment 4 — POS & Parsing**  
spaCy POS tags, dependency parses, noun chunks; intro to constituency trees; CRF vs. HMM (concept).

**Assignment 5 — Text Summarization**  
Extractive (TextRank/Lead-k/frequency) vs. small abstractive summarizers; brief ROUGE overview.

**Assignment 6 — Story Generation**  
Simple Markov chain text generation and a small local language model for short stories.

**Assignment 7 — Article Analysis (VentureBeat)**  
LLM summary; key topics; sentiment (LLM vs. NB/SVM); emotion; and main theme detection.

**Assignment 8 — Cross-Outlet Comparison**  
Two climate articles: semantic similarity, top keywords, sentiment & emotion profiles, concise summaries.

**Assignment 9 — News Classification**  
AP article: sentiment, intent, and emotion; simple domain/topic proportions; compare LLM vs. DL sentiment.

**Assignment 10 — Topics & Clustering**  
LDA/LSI on chunks, hierarchical clustering of topic vectors, top keywords, and a brief summary.

---

## 3) Tech Stack

**Libraries / Frameworks**
- Python, Jupyter Notebooks  
- pandas, numpy, matplotlib / seaborn  
- requests, beautifulsoup4 (web scraping)  
- NLTK, spaCy, benepar (linguistics & parsing)  
- scikit-learn (TF-IDF, classifiers, clustering, evaluation)  
- sentence-transformers (sentence embeddings)  
- transformers (summarization & small LMs)  
- gensim (LDA/LSI topic modeling)

**Models**
- spaCy: `en_core_web_sm`  
- benepar: `benepar_en3`  
- Sentence-Transformers: `all-MiniLM-L6-v2`  
- Abstractive summarization: `sshleifer/distilbart-cnn-12-6`  
- Language model (toy): `distilgpt2`  
- Sentiment baseline: `distilbert-base-uncased-finetuned-sst-2-english`

---

## 4) Overview of Files

These assignments walk through the end-to-end NLP pipeline: web data collection, text cleaning/normalization, feature engineering (BoW/TF-IDF), and classic modeling (similarity, classification). You’ll also cover linguistic analysis (POS, dependencies), summarization (extractive/abstractive), embeddings and semantic search, topic modeling/clustering, and applied sentiment/emotion/intent analysis—culminating in practical, reproducible NLP workflows.

