# RFM Customer Segmentation Analysis

## Project Overview
This project performs **RFM (Recency, Frequency, Monetary) Analysis** to segment customers based on their purchasing behavior. RFM analysis is a widely used customer analytics technique in marketing and retail to identify high-value customers and understand customer engagement.

By analyzing transaction data, the project classifies customers into segments such as **Champions, Potential Loyalists, At-Risk Customers, and Lost Customers**, helping businesses design targeted marketing strategies.

---

## Objectives

- Calculate **Recency, Frequency, and Monetary values** for each customer
- Generate **RFM scores** to measure customer engagement
- Segment customers based on their purchasing behavior
- Identify **high-value and at-risk customers**
- Visualize customer segments and behavioral patterns

---

## Dataset

The dataset contains customer transaction information with the following fields:

- **CustomerID** – Unique identifier for each customer
- **PurchaseDate** – Date of purchase
- **TransactionAmount** – Amount spent in the transaction
- **ProductInformation** – Product details
- **OrderID** – Order identifier
- **Location** – Customer location

---

## Technologies Used

- Python
- Pandas
- Plotly
- Plotly Express
- Data Visualization
- Customer Analytics

---

## Methodology

### 1. Data Preprocessing
- Converted purchase date into datetime format
- Cleaned and structured transaction data for analysis

### 2. RFM Metric Calculation

**Recency**
- Number of days since the customer’s last purchase

**Frequency**
- Total number of purchases made by the customer

**Monetary**
- Total amount spent by the customer

### 3. RFM Score Calculation

Each metric was assigned a score from **1 to 5** based on value ranges.

- **Recency Score** – Higher score for more recent purchases
- **Frequency Score** – Higher score for frequent purchases
- **Monetary Score** – Higher score for higher spending

The final **RFM Score** was calculated as:

RFM Score = Recency Score + Frequency Score + Monetary Score

---

### 4. Customer Segmentation

Customers were categorized into the following segments:

| Segment | Description |
|------|------|
| Champions | Highly engaged customers with frequent purchases and high spending |
| Potential Loyalists | Customers with strong engagement potential |
| At Risk Customers | Customers whose engagement is declining |
| Can't Lose | Previously valuable customers at risk of churn |
| Lost | Customers with very low engagement |

---

## Visualizations

The project includes several visual analytics:

- **RFM Value Segment Distribution**
- **Treemap of Customer Segments**
- **Distribution of RFM Scores for Champions**
- **Correlation Heatmap of RFM Metrics**
- **Segment Comparison Bar Charts**
- **Average RFM Scores by Segment**

These visualizations help understand **customer behavior patterns and segment characteristics**.

---

## Key Insights

- **Champions segment** represents highly valuable customers with strong purchase frequency and spending behavior.
- **Potential Loyalists** represent an opportunity for targeted marketing campaigns.
- **At-risk and lost customers** highlight areas where retention strategies may be needed.
- RFM segmentation enables businesses to prioritize marketing resources effectively.

---

## Repository Structure

```
RFM-Customer-Segmentation-Analysis
│
├── data
│   └── rfm_data.csv
│
├── notebooks
│   └── rfm_customer_segmentation.ipynb
│
├── images
│   ├── segment_distribution.png
│   ├── rfm_treemap.png
│   ├── champions_distribution.png
│   ├── correlation_heatmap.png
│   └── segment_comparison.png
│
├── requirements.txt
└── README.md
```

---

## Future Improvements

Possible extensions for this project include:

- Applying **machine learning clustering algorithms** such as K-Means for customer segmentation
- Building **customer lifetime value (CLV) prediction models**
- Creating an **interactive marketing dashboard**
- Integrating RFM analysis into **real-time customer analytics pipelines**
