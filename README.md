# IMDB Sentiment Classification – NLP Course Project

A tiny NLP project that trains a Logistic Regression model to classify movie reviews as positive or negative.  
Dataset: `imdb_labelled.txt` (sentence-level labels, 0 = negative, 1 = positive).

## What it does
- Loads the labelled sentences.
- Splits them into 80% training / 20% validation (stratified).
- Converts text to numerical features using TF‑IDF.
- Trains a Logistic Regression classifier.
- Evaluates on the validation set and prints accuracy, classification report, and confusion matrix.
- Predicts sentiment for a few brand‑new sentences.

## Results
Validation accuracy: **~77%**  


## Tech used
- Python 3
- Pandas, NumPy
- Scikit‑learn (train_test_split, TfidfVectorizer, LogisticRegression, metrics)
- Jupyter Notebook

## How to run it

1. Clone this repo or download the files.
2. Create a virtual environment (optional but nice):
   ```bash
   python -m venv nlp_env
   nlp_env\Scripts\activate      # Windows
   source nlp_env/bin/activate   # Mac/Linux