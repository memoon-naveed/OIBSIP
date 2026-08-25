# Demo Video, LinkedIn, and Submission Guide

## 1. Required Two-Second Title Card

Display this text clearly for at least two seconds before the walkthrough begins:

```text
Memoon Naveed
Assigned Track: Data Analytics
Task 3: Professional Data Cleaning
```

Use `screenshots/00_demo_title_card.png` as the opening frame and keep it visible for at least two seconds.

## 2. Recommended Demo Length

Keep the walkthrough between **90 seconds and 2 minutes**. Record at 1080p if possible and ensure notebook text remains readable.

## 3. Demo Recording Sequence and Narration

### 0:00–0:02 — Title card

Show the required title card without movement.

### 0:02–0:12 — Project introduction

> Hello, I am Memoon Naveed. This is my Data Analytics Task 3 for Oasis Infobyte. In this project, I transformed a deliberately messy employee dataset into a validated, analysis-ready dataset using Python, pandas, and NumPy.

Show the repository folder and open the notebook.

### 0:12–0:28 — Raw dataset and quality report

> The original dataset contains 1,020 rows and 12 columns. I created a professional data-quality report that checks explicit and hidden missing values, duplicate rows, unique values, incorrect data types, and format or range anomalies.

Show the raw preview, `df.info()`, null counts, and the initial quality-report table.

### 0:28–0:52 — Cleaning decisions

> I documented a separate missing-value strategy for each column. Age and salary use department-aware median imputation, categorical fields use mode where appropriate, and missing contact information is retained rather than fabricated. I also standardized employee IDs, names, categories, mixed date formats, emails, and phone numbers.

Scroll through the Markdown decision table and key cleaning cells.

### 0:52–1:08 — Outliers and duplicates

> I used the IQR method to identify numeric outliers and documented whether each type should be retained or capped. I then removed exact duplicates and duplicate person records using a carefully defined business key.

Show the IQR explanation, outlier summary, and duplicate-removal output.

### 1:08–1:28 — Before and after

> After cleaning, format and range anomalies decreased from 92 to zero, target data-type accuracy improved from 16.7 percent to 100 percent, and the final dataset contains 1,014 rows and 13 structured columns.

Show `screenshots/02_before_after_quality_summary.png` or the equivalent notebook output.

### 1:28–1:45 — Validation and export

> Finally, I ran nine automated quality checks covering unique IDs, valid ages, positive salaries, dates, categories, duplicates, and data types. All nine checks passed, and the clean dataset was exported as a new CSV file.

Show the validation table, the export message, and the cleaned CSV file in the folder.

### Closing

> This project demonstrated that professional data cleaning requires documented, defensible decisions—not simply deleting every incomplete row. Thank you for watching.

## 4. GitHub Commands

Repository: `https://github.com/memoon-naveed/OIBSIP.git`

Run these commands from the root of the existing `OIBSIP` repository after placing the project folder inside it:

```bash
git status
git add DataAnalytics-Task3-ProfessionalDataCleaning
git commit -m "Complete Task 3 professional data cleaning project"
git push origin main
```

If your default branch is `master`, replace `main` with `master`.

## 5. LinkedIn Post

Replace the GitHub and demo links before publishing. Type `@Oasis Infobyte` inside LinkedIn and select the official company page so the tag becomes active.

```text
I completed Task 3 of my Data Analytics internship with Oasis Infobyte: Professional Data Cleaning using Python.

The project transformed a deliberately messy employee dataset into a validated, analysis-ready CSV.

Key results:
• Analysed 1,020 raw employee records
• Reduced effective missing values from 235 to 91 intentional missing contact values
• Resolved 92 format and range anomalies
• Improved target data-type accuracy from 16.7% to 100%
• Standardized IDs, categories, dates, emails, and phone numbers
• Applied department-aware median and categorical mode imputation
• Used the IQR method for outlier analysis
• Removed six duplicate person records
• Passed all 9 automated data-quality checks

Tech stack: Python, pandas, NumPy, matplotlib, seaborn, and Jupyter Notebook.

GitHub: [PASTE GITHUB PROJECT LINK]
Demo video: [PASTE VIDEO LINK IF NEEDED]

Thank you @Oasis Infobyte for the opportunity to apply professional data-cleaning techniques to a practical dataset.

#oasisinfobyte #dataanalytics #python #pandas #numpy #datacleaning #datascience #internship
```

## 6. Substantive Peer-Evaluation Comments

Personalize these comments after watching each intern's complete demo.

### Comment 1

> I liked how you implemented **[specific feature]**, especially the way you **[specific observation from their demo]**. Your explanation made the workflow easy to follow. Did you consider **[relevant technical question or alternative]**? I would be interested to know how that choice affected the final result.

### Comment 2

> Your demonstration of **[specific technique or visualization]** was clear and practical. One detail that stood out was **[specific implementation detail]**. A possible enhancement could be **[constructive suggestion]**, although the current implementation already communicates the result effectively.

Do not post the templates without replacing every bracketed field.

## 7. Final Submission Checklist

- [ ] Folder name exactly matches `DataAnalytics-Task3-ProfessionalDataCleaning`
- [ ] Notebook runs from beginning to end
- [ ] Cleaned CSV exists
- [ ] README and screenshots are visible on GitHub
- [ ] Demo starts with the required two-second title card
- [ ] Demo shows the complete functioning workflow
- [ ] LinkedIn post tags Oasis Infobyte
- [ ] LinkedIn post contains `#oasisinfobyte`
- [ ] Two substantive peer comments are published
- [ ] GitHub project link is entered in the submission form
- [ ] Submission form is reviewed before final submission
