# Retail Sales Exploratory Data Analysis — Task 1

An end-to-end exploratory data analysis of 102,771 retail transactions. The project examines sales trends, customer demographics, product performance, correlations, and seasonal buying behaviour, then converts the findings into practical business recommendations.

## Internship details

- **Intern:** Memoon Naveed
- **Track:** Data Analytics
- **Organization:** Oasis Infobyte
- **Task:** Task 1 — EDA on Retail Sales Data

## Dataset

This project uses the [Customer Behavior and Purchase Dataset](https://www.kaggle.com/datasets/timcii/clothing-store-sales-data/data) published on Kaggle under the CC BY-SA 4.0 licence.

- 102,771 transaction rows and 21 source columns
- Coverage: January 2022 through December 2024
- 3,900 unique customers
- Customer, product, transaction, date, promotion, rating, and churn attributes

`retail_sales.csv` is included so the notebook can be run without downloading anything else. The source file uses a semicolon delimiter, which is handled in the notebook.

## Analysis completed

- Initial inspection: shape, data types, missing values, and duplicates
- Descriptive statistics: mean, median, mode, and standard deviation
- Monthly and quarterly revenue trends
- Unique-customer age group and gender analysis
- Best-selling products and category revenue
- Correlation heatmap for numerical variables
- Additional seasonal volume-versus-value analysis
- Written observations after every visualisation
- Five actionable business recommendations and limitations

## Verified highlights

| Metric | Result |
|---|---:|
| Total revenue | $5,331,988.70 |
| Average transaction | $51.88 |
| Highest-revenue month | December 2024 — $284,590.40 |
| Highest-revenue quarter | Q4 2024 — $645,748.10 |
| Best-selling product | Sweater — 43,661 transactions |
| Leading category | Clothing — $3,591,140.70 (67.35%) |
| Highest-volume season | Summer — 29,321 transactions |
| Highest average transaction season | Winter — $56.53 |

## Key business insights

1. Revenue rose strongly over the three-year period, and Q4 was the peak quarter in every year. Inventory, fulfilment capacity, and campaigns should be ready before the year-end surge.
2. Sweaters and the Clothing category dominate sales. Protecting their availability is essential, while bundles can cross-sell lower-share categories.
3. Summer produces the most transactions but the lowest average transaction value; basket-building offers are more suitable than broad discounts. Winter has fewer transactions but the highest average value, which supports premium positioning.
4. Men represent 68% of unique customers. This protects a strong existing segment but also reveals an opportunity to grow the underrepresented female customer base through targeted acquisition and assortment testing.
5. Customers aged 55–64 contribute the most revenue, while the 65+ group has the highest average spend. Retention and accessible shopping experiences should be prioritised for older customers.

## Project structure

```text
OIBSIP/
└── DataAnalytics-Task1-EDARetailSales/
    ├── Task_1_Retail_Sales_EDA.ipynb
    ├── retail_sales.csv
    ├── descriptive_statistics.csv
    ├── eda_key_metrics.csv
    ├── monthly_sales.csv
    ├── quarterly_sales.csv
    ├── customer_age_group_distribution.csv
    ├── top_products.csv
    ├── category_revenue.csv
    ├── seasonal_sales_summary.csv
    ├── screenshots/
    │   ├── 00_demo_title_card.png
    │   ├── 01_monthly_quarterly_sales_trends.png
    │   ├── 02_customer_demographics.png
    │   ├── 03_product_category_performance.png
    │   ├── 04_correlation_heatmap.png
    │   └── 05_seasonal_volume_value_insight.png
    ├── DEMO_AND_SUBMISSION_GUIDE.md
    ├── requirements.txt
    ├── .gitignore
    └── README.md
```

## How to run

1. Clone the repository and open this project folder.
2. Create and activate a Python environment.
3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `Task_1_Retail_Sales_EDA.ipynb` and select **Run All**.

The submitted notebook is already executed, so all tables, observations, and charts are visible immediately on GitHub.

## Limitations

- Each record is treated as one item-level transaction because the dataset has no quantity field.
- Revenue is analysed without cost or profit data, so recommendations should be validated against margins.
- Correlation describes association, not causation.
- The dataset is suitable for analytical practice; conclusions should be validated with live operational data before production use.

## Author

**Memoon Naveed**  
Data Analytics Intern — Oasis Infobyte
