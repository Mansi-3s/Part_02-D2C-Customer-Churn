# Customer Segmentation and Retention Strategy Analysis

## Project Overview

This project performs customer segmentation using RFM (Recency, Frequency, Monetary) analysis and develops actionable retention strategies for each customer segment. The objective is to identify valuable customers, detect churn risks, and recommend targeted business interventions to improve customer retention and lifetime value.

---

## Dataset

The dataset contains customer transaction, engagement, and support interaction information, including:

* Customer ID
* Purchase history
* Revenue generated
* Recency of purchases
* Website/App engagement metrics
* Support ticket information
* Churn labels (where applicable)

---

## Project Objectives

1. Perform customer segmentation using RFM analysis.
2. Identify high-value and at-risk customers.
3. Develop retention strategies for each segment.
4. Prioritize marketing budget allocation.
5. Conduct manual review of ambiguous customer cases.
6. Generate business-ready recommendations.

---

## Methodology

### 1. Data Preprocessing

* Missing value handling
* Feature engineering
* Date conversion
* Customer-level aggregation

### 2. RFM Analysis

Three key metrics were calculated:

* **Recency (R):** Days since last purchase
* **Frequency (F):** Number of purchases
* **Monetary (M):** Total spending

Customers were scored and grouped into meaningful business segments.

### 3. Customer Segmentation

Customers were categorized into:

* Loyal Customers
* Potential Loyalists
* New Customers
* At Risk Customers
* Dormant Customers

### 4. Business Analysis

Additional analyses included:

* Segment revenue contribution
* Segment churn behavior
* Customer engagement patterns
* Support ticket analysis

### 5. Manual Review Cases

Ten customers with conflicting behavioral signals were manually reviewed.

Examples of conflicting signals:

* High spending but no engagement
* Strong purchase history but customer complaints
* Dormant customers with unusually high revenue
* Loyal customers showing inactivity trends

---

## Retention Strategy

### Loyal Customers

* Loyalty rewards
* VIP programs
* Cross-selling opportunities

### Potential Loyalists

* Personalized recommendations
* Repeat purchase incentives

### At Risk Customers

* Reactivation campaigns
* Discount offers
* Customer outreach

### Dormant Customers

* Win-back campaigns
* Personalized promotions

### High Value but Unhappy Customers

* Immediate customer success intervention
* Service recovery actions

---

## Output Files

All generated outputs are saved in the `output/` directory.

### Generated Files

| File                        | Description                     |
| --------------------------- | ------------------------------- |
| segments.csv                | Customer segment assignments    |
| segment_summary.csv         | Segment statistics              |
| segment_churn.csv           | Churn analysis by segment       |
| segment_revenue.csv         | Revenue contribution by segment |
| retention_actions.csv       | Recommended retention actions   |
| manual_review_customers.csv | Manual review customer cases    |
| budget_allocation.csv       | Marketing budget prioritization |

---

## Project Structure

```text
project/
│
├── rfm_segmentation.ipynb
├── requirements.txt
├── README.md
│
└── output/
    ├── segments.csv
    ├── segment_summary.csv
    ├── segment_churn.csv
    ├── segment_revenue.csv
    ├── retention_actions.csv
    ├── manual_review_customers.csv
    └── budget_allocation.csv
```

---
## Installation

### 1. Clone the repository

```bash
git clone https://github.com/Mansi-3s/Part_02-D2C-Customer-Churn.git
cd Part 2: RFM Segmentation & Retention Strategy

---

## Running the Project

Execute the notebook:

```bash
## Install dependencies

pip install -r requirements.txt

jupyter notebook rfm_segmentation.ipynb
```

Run all cells sequentially to generate the segmentation analysis and output files.

---

## Key Findings

* Loyal customers contribute the highest revenue.
* Several high-value customers show low engagement and require monitoring.
* Support ticket sentiment can reveal hidden churn risks.
* Dormant customers may still represent significant reactivation opportunities.
* Manual review improves decision quality for edge cases that automated segmentation may misclassify.

---

## Business Impact

The project enables data-driven customer retention by:

* Identifying valuable customer groups
* Prioritizing marketing efforts
* Reducing churn risk
* Improving customer lifetime value
* Supporting strategic decision-making

---
