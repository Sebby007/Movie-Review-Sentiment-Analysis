Movie Review Sentiment Analysis with Classical NLP and BERT
In this project, I developed a sentiment analysis system for automatically classifying movie reviews as positive or negative using the IMDB reviews dataset. The goal was to build a reliable text-classification model achieving an F1 score ≥ 0.85, while also evaluating trade-offs between model complexity, performance, and computational cost.

🔍 Project Workflow

Loaded and explored labeled IMDB movie reviews

Performed text preprocessing and EDA to assess class balance

Transformed text using multiple vectorization strategies:

TF-IDF (1–2 n-grams)

TF-IDF with spaCy normalization (lemmatization, stopword removal)

BERT embeddings (subset due to computational cost)

Trained and evaluated multiple models:

Dummy baseline

Logistic Regression

LightGBM

Logistic Regression on BERT embeddings

Tuned classification thresholds to maximize F1 score rather than using a fixed 0.5 cutoff

📊 Key Results

TF-IDF + Logistic Regression delivered the best balance of accuracy, speed, and simplicity

spaCy normalization provided a small but consistent performance boost

BERT embeddings achieved comparable accuracy but were significantly more computationally expensive

Gradient boosting did not outperform simpler linear models in this task

✅ Conclusion

A well-tuned classical NLP pipeline can match or exceed deep-learning approaches for many real-world text classification tasks, while remaining faster, cheaper, and easier to deploy. This project highlights the importance of model selection based on business constraints, not just raw accuracy.
