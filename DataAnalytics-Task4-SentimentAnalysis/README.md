# Sentiment Analysis — Task 4

Machine-learning project that classifies airline-related tweets as **negative**, **neutral**, or **positive**. The workflow covers data inspection, NLP preprocessing, TF-IDF feature extraction, two classifiers, complete evaluation, visualisation, and error analysis.

## Task Information

- **Intern:** Memoon Naveed
- **Assigned Track:** Data Analytics
- **Task:** Task 4 — Sentiment Analysis
- **Organisation:** Oasis Infobyte
- **Tech stack:** Python, pandas, scikit-learn, NLTK, matplotlib, seaborn, WordCloud, Jupyter Notebook

## Dataset

The project uses the Kaggle **US Airline Twitter Sentiment Analysis Dataset**. It contains 14,640 tweets and three target classes. The included source file is `Tweets.csv`.

- Dataset page: https://www.kaggle.com/datasets/zahranusratt/us-airline-twitter-sentiment-analysis-dataset
- Source licence shown on Kaggle: CC0 — Public Domain
- Target column: `airline_sentiment`
- Text column: `text`

## Workflow

1. Load the CSV and inspect schema, missing values, duplicates, and labels.
2. Keep the text and sentiment fields, remove unusable rows, and normalise labels.
3. Lowercase text, remove URLs, mentions, punctuation, and stopwords, then tokenise and lemmatise with NLTK.
4. Plot class distribution and generate a WordCloud for every sentiment class.
5. Create an 80/20 stratified train/test split.
6. transform cleaned text into TF-IDF unigram and bigram features.
7. Train Multinomial Naive Bayes and Logistic Regression.
8. Compare accuracy, macro precision, macro recall, macro F1, classification reports, and confusion matrices.
9. Inspect five high-confidence misclassifications and discuss likely causes.
10. Select the best model and explain real-world applications and limitations.

## Verified Results

| Model | Accuracy | Macro Precision | Macro Recall | Macro F1 |
|---|---:|---:|---:|---:|
| Logistic Regression | **0.7988** | 0.7734 | **0.7020** | **0.7298** |
| Multinomial Naive Bayes | 0.7432 | **0.7993** | 0.5589 | 0.6037 |

**Best model:** Logistic Regression. It offered the best overall balance across the three unequal classes, improving macro F1 by 0.1261 over Naive Bayes.

The final cleaned modelling set contained 14,408 usable tweets. The stratified split produced 11,526 training examples and 2,882 test examples. Logistic Regression misclassified 580 test examples, giving a 20.12% test error rate.

## Main Findings

- Negative tweets dominate the dataset, representing roughly 63% of usable records.
- Naive Bayes strongly favoured the majority negative class and had weak neutral/positive recall.
- Logistic Regression substantially improved minority-class recognition while retaining strong negative-class performance.
- Common errors involved short replies, mixed sentiment, sarcasm, missing conversation context, and ambiguous neutral/positive boundaries.
- The model can support customer-feedback monitoring, support-ticket triage, airline service analysis, and public-opinion tracking.

## Repository Structure

```text
DataAnalytics-Task4-SentimentAnalysis/
├── Task_4_Sentiment_Analysis.ipynb
├── Tweets.csv
├── model_metrics.csv
├── misclassified_examples.csv
├── requirements.txt
├── README.md
├── DEMO_AND_SUBMISSION_GUIDE.md
└── screenshots/
    ├── 00_demo_title_card.png
    ├── 01_sentiment_distribution.png
    ├── 02_wordclouds_by_sentiment.png
    ├── 03_confusion_matrices.png
    ├── 04_model_performance_comparison.png
    └── 05_error_patterns.png
```

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook Task_4_Sentiment_Analysis.ipynb
```

Run all cells in order. The notebook uses a fixed random seed and automatically reads `Tweets.csv` from the project folder.

## Limitations

- Tweets are short, informal, and sometimes sarcastic.
- TF-IDF represents term importance but not full syntax or conversational context.
- The dataset is imbalanced toward negative sentiment.
- Performance may decline on another platform, industry, language, or time period.

Future improvements could include class weighting, hyperparameter tuning, character n-grams, a linear SVM, emoji-aware preprocessing, or a contextual model such as BERT.

## Author

**Memoon Naveed**  
Data Analytics Intern — Oasis Infobyte

