# generate_readme.py
from datetime import datetime
from pathlib import Path

COURSE_NOTE = (
    "These are my **NLP Assignments** for my course **Data 622 — Natural Language Processing** "
    "in my **3rd semester class at UMBC**, taught by **Prof. Tony Diana**."
)

ASSIGNMENTS = [
    {
        "title": "HW1 — Web Scraping Basics",
        "desc": "Requests + BeautifulSoup to fetch pages, extract visible text/headings/links, and save snippets."
    },
    {
        "title": "HW2 — Text Cleaning & Normalization",
        "desc": "Lowercasing, punctuation/HTML stripping, stopword removal, stemming vs lemmatization; clean corpora for modeling."
    },
    {
        "title": "HW3 — Similarity & Embeddings",
        "desc": "Compare TF-IDF cosine vs sentence embeddings; compute sentence/document similarity for retrieval."
    },
    {
        "title": "HW4 — POS & Parsing",
        "desc": "spaCy POS tagging, dependency parsing, noun chunks; intro to constituency trees and CRF vs HMM conceptually."
    },
    {
        "title": "HW5 — Text Summarization",
        "desc": "Extractive (TextRank/Lead-k/frequency) and small-model abstractive summaries; compare outputs."
    },
    {
        "title": "HW6 — Story Generation",
        "desc": "Simple Markov chain generation and small local LM generation; prompt/temperature basics."
    },
    {
        "title": "HW7 — Article Analysis (VentureBeat)",
        "desc": "LLM summary; key topics; sentiment (LLM vs NB/SVM); emotion; and main theme extraction."
    },
    {
        "title": "HW8 — Cross-Outlet Comparison",
        "desc": "Two climate articles: semantic similarity, top keywords, sentiment & emotion profiling, concise summaries."
    },
    {
        "title": "HW9 — News Classification",
        "desc": "AP article: sentiment, intent, emotion; simple domain/topic proportions; compare LLM vs DL sentiment."
    },
    {
        "title": "HW10 — Topics & Clustering",
        "desc": "LDA/LSI topic modeling on chunks, hierarchical clustering of topic vectors, top keywords, brief summary."
    },
]

README = f"""# 📚 DATA 622 — NLP Assignments (UMBC)

> **Author:** Soumya Bhate  
> **Course:** Data 622 — Natural Language Processing (3rd Semester, UMBC)  
> **Instructor:** Prof. Tony Diana

{COURSE_NOTE}

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![NLP](https://img.shields.io/badge/NLP-Data622-green)
![Jupyter](https://img.shields.io/badge/Notebooks-Yes-informational)
![License](https://img.shields.io/badge/Repo-Student%20Work-lightgrey)

---

## 🔎 Table of Contents
{chr(10).join(f"- [{i+1}. {a['title']}](#hw{i+1}-{a['title'].lower().replace('—','').replace(' ','-').replace('&','and')})" for i,a in enumerate(ASSIGNMENTS))}

---

## 🧭 Overview
{COURSE_NOTE}

Each homework folder contains notebooks and/or scripts demonstrating the concepts below.  
Short descriptions for quick navigation:

{"".join(f"### HW{i+1}. {a['title']}\n{a['desc']}\n\n" for i,a in enumerate(ASSIGNMENTS))}\
## 🚀 Getting Started
```bash
git clone <your-repo-url>.git
cd <repo>
# (optional) create a virtual environment
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\\Scripts\\activate
# install per-notebook requirements as needed
