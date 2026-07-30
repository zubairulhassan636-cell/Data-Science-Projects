# DecodeLabs Project 4 — NLP & Sentiment Analysis

## Objective
Build an NLP pipeline that converts unstructured product reviews into numerical TF-IDF features and predicts Positive/Negative sentiment.

## Requirements covered
- Tokenization with NLTK
- Stop-word removal while preserving negations such as `not`, `no`, and `never`
- NLTK WordNetLemmatizer
- POS-guided lemmatization
- TF-IDF vectorization
- Unigrams + bigrams
- `max_features=10000` and `min_df=2`
- SciPy CSR sparse matrices
- Multinomial Naive Bayes
- Laplace smoothing with `alpha=1.0`
- Accuracy, classification report, confusion matrix
- Prediction of new reviews
- Optional comparison with ComplementNB
- Error analysis

## Files
- `NLP_Sentiment_Analysis_Project4.ipynb` — complete project notebook
- `product_reviews.csv` — balanced educational product-review dataset
- `requirements.txt` — required Python packages

## How to run
1. Open the folder in VS Code, Jupyter Notebook, or JupyterLab.
2. Install dependencies:
   `pip install -r requirements.txt`
3. Open `NLP_Sentiment_Analysis_Project4.ipynb`.
4. Run all cells from top to bottom.
5. The notebook downloads the required NLTK language resources the first time it is run.

## Dataset note
The CSV is a curated educational dataset created for this project so the submission is self-contained and does not depend on an external dataset URL.
