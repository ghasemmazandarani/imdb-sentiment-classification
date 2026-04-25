# IMDB Sentiment Classification – NLP Course Project

A small NLP project that classifies movie reviews as **positive** or **negative** using Logistic Regression.  
The dataset (`imdb_labelled.txt`) contains 748 labelled sentences.

Two feature extraction methods are compared:

- **TF‑IDF** → notebook `imdb_sentiment_classifier.ipynb`
- **Bag of Words (CountVectorizer)** → notebook `imdb_sentiment_bow.ipynb`

Both approaches follow the same pipeline: load → split (80/20 stratified) → vectorize → train → evaluate.

---

## Results

| Method       | Validation Accuracy |
|--------------|---------------------|
| TF‑IDF       | 76.67%              |
| Bag of Words | 77.33%              |

The small difference is normal for this dataset size. Both models perform reasonably well for a simple baseline.

---

## What the notebooks do

- Read the labelled sentences from `imdb_labelled.txt`
- Split into training (80%) and validation (20%) sets
- Convert text to numerical features (TF‑IDF or CountVectorizer)
- Train a Logistic Regression classifier
- Print accuracy, classification report, and confusion matrix

---

## Tech stack

- Python 3
- Pandas, NumPy
- Scikit‑learn (`train_test_split`, `TfidfVectorizer`, `CountVectorizer`, `LogisticRegression`)
- Jupyter Notebook

---

## How to run

1. Clone this repo or download the files.
2. (Optional) Create and activate a virtual environment:
   ```bash
   python -m venv nlp_env
   nlp_env\Scripts\activate      # Windows
   source nlp_env/bin/activate   # Mac/Linux