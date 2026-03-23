# Reddit NSFW Classification using NLP & Machine Learning

## Project Overview
This project builds a Machine Learning model to classify Reddit posts as **NSFW (Not Safe For Work)** or **Safe** using Natural Language Processing (NLP).

The system analyzes post titles and predicts whether the content is adult or appropriate, helping automate **content moderation**.

---

## Dataset
- Source: Reddit posts dataset (`r_dataisbeautiful_posts.csv`)
- Size: ~193,000 posts
- Key Features:
  - `title` → Text data (main feature)
  - `score` → Post engagement
  - `num_comments`
  - `over_18` → Target variable (NSFW label)

---

## Problem Statement
With large-scale user-generated content, manual moderation is inefficient.

 Goal: Build an automated system to detect NSFW content using Machine Learning.

---

## ⚙️ Tech Stack
- Python
- Pandas, NumPy
- NLTK, spaCy
- Scikit-learn
- Matplotlib, Seaborn
- PandasQL

---

## Workflow

### 1. Data Exploration
- Loaded and analyzed dataset (~193K rows)
- Checked missing values and distributions

### 2. Data Preprocessing
- Text cleaning (lowercasing, removing special characters)
- Stopword removal (NLTK)
- Tokenization

### 3. Feature Engineering
- Converted text into numerical vectors using **TF-IDF**

### 4. Model Training
- Decision Tree Classifier
- Random Forest Classifier (Best performing)

### 5. Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score

---

## Results
- Achieved high performance with Random Forest
- Balanced precision and recall for classification

```text
Accuracy: ~91%
Precision: 0.91
Recall: 0.89
F1 Score: 0.90
