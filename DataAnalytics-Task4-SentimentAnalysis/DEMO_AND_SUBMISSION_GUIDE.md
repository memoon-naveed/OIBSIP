# Demo, LinkedIn, and Submission Guide

## 1. GitHub Folder

Upload this complete folder to:

`OIBSIP/DataAnalytics-Task4-SentimentAnalysis/`

Repository: https://github.com/memoon-naveed/OIBSIP

Suggested commit message:

`Add Task 4 sentiment analysis project`

## 2. Demo Video Structure

Aim for a clear 2–4 minute screen recording.

### Required opening — 2 seconds

Display `screenshots/00_demo_title_card.png` for at least two seconds. It contains:

- Memoon Naveed
- Assigned Track: Data Analytics
- Task 4: Sentiment Analysis

### Walkthrough

1. **Introduction:** “Hello, I am Memoon Naveed. This is Task 4, Sentiment Analysis, for my Data Analytics internship at Oasis Infobyte.”
2. **Dataset:** Show `Tweets.csv`, its 14,640 rows, and the positive/neutral/negative labels.
3. **Distribution:** Explain that negative feedback is the majority class.
4. **Preprocessing:** Show lowercasing, URL/mention/punctuation removal, tokenisation, stopword removal, and lemmatisation.
5. **TF-IDF:** Explain that TF-IDF converts text into numerical features and gives more importance to informative terms.
6. **Split and models:** Show the stratified 80/20 split, Multinomial Naive Bayes, and Logistic Regression.
7. **Evaluation:** Show the metrics table and both confusion matrices.
8. **WordClouds:** Briefly compare the prominent words in each class.
9. **Errors:** Show the five misclassified examples and explain short context, mixed sentiment, sarcasm, and ambiguous labels.
10. **Conclusion:** State that Logistic Regression performed best with 79.88% accuracy and 0.7298 macro F1.

End by showing the GitHub repository folder.

## 3. LinkedIn Post

I am excited to share **Task 4 — Sentiment Analysis**, completed as part of my Data Analytics internship with **Oasis Infobyte**.

For this project, I built a machine-learning pipeline that classifies airline-related tweets as positive, negative, or neutral. I cleaned and tokenised the text, removed stopwords, used TF-IDF feature extraction, and compared Multinomial Naive Bayes with Logistic Regression.

The project includes class-distribution analysis, WordClouds, classification reports, confusion matrices, and a detailed review of five misclassified tweets. Logistic Regression performed best, achieving **79.88% accuracy** and a **0.7298 macro F1-score**.

This solution could support customer-feedback monitoring, support-ticket prioritisation, brand tracking, and public-opinion analysis.

GitHub: https://github.com/memoon-naveed/OIBSIP

@Oasis Infobyte

#oasisinfobyte #datascience #dataanalytics #python #machinelearning #nlp #sentimentanalysis #internship

## 4. Peer Evaluation Examples

Leave substantive comments on at least two interns’ posts. Personalise these examples before posting:

1. “Your preprocessing workflow is clearly structured, especially the way you handled noisy text. Did you compare how the model performed before and after stopword removal?”
2. “The confusion matrix makes the model’s class-level behaviour easy to understand. It would be interesting to know whether class weighting improved the minority-class recall.”

## 5. Submission Checklist

- [ ] Complete project folder uploaded to the `OIBSIP` repository
- [ ] README visible on GitHub
- [ ] Notebook, dataset, outputs, and screenshots included
- [ ] Demo begins with the required two-second title card
- [ ] End-to-end notebook workflow shown in the video
- [ ] LinkedIn post tags Oasis Infobyte
- [ ] `#oasisinfobyte` included
- [ ] Two substantive peer-evaluation comments completed
- [ ] Submission form includes the GitHub repository link

