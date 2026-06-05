# Supply Chain Performance Analytics

Exploratory Data Analysis (EDA) on a global supply chain dataset to identify operational inefficiencies, quantify revenue at risk from late deliveries, and surface actionable business insights across shipping modes, markets, regions, and product categories.

---

## Overview

Late deliveries are one of the most measurable operational failures in supply chain management — they directly impact customer satisfaction, cancellation rates, and recoverable revenue. This project uses Python-based EDA to systematically diagnose where delays are concentrated, how much revenue is at risk, and which operational levers have the highest impact.

**Dataset:** 180,000+ order records across 53 columns including order dates, shipping dates, markets, regions, product categories, customer segments, and financial metrics.

---

## Business Questions Answered

- Which shipping modes have the highest late delivery risk — and by how much versus the global average?
- Which markets and regions consistently underperform on delivery?
- What is the total revenue at risk from late deliveries, and which product categories drive the most exposure?
- Which route combinations (region × shipping mode) are the worst performers?
- How does late delivery risk vary by customer segment, order type, and department?
- Are there seasonal patterns in delivery failures?

---

## Key Analyses

### 1. Delivery Delay Index (DDI)

Created a custom metric:

```text
DDI = Actual Shipping Days − Scheduled Shipping Days
```

Used alongside a high-risk delivery flag to identify significant delivery failures.

### 2. Late Delivery Risk by Shipping Mode

Grouped late delivery risk rates by shipping mode and benchmarked each against the global average.

### 3. Market & Regional Analysis

Computed late delivery rates, average delay severity, and total order volume across markets and regions.

### 4. Revenue at Risk by Product Category

Calculated revenue exposure associated with delayed deliveries and ranked product categories by financial impact.

### 5. Route-Level Analysis

Created a composite route variable using:

```text
Region + Shipping Mode
```

to identify the highest-risk operational routes.

### 6. Customer Segment & Order Type Analysis

Compared delay risk across:

- Customer Segments
- Single-item Orders
- Bulk Orders

### 7. Seasonal Trend Analysis

Analyzed monthly delivery patterns to identify operational stress periods and seasonal spikes.

### 8. Order Status & Payment Type Analysis

Evaluated relationships between:

- Payment Methods
- Order Completion
- Cancellations
- Delivery Outcomes

---

## Key Insights

- First Class shipping recorded the highest frequency of late deliveries.
- Second Class shipping exhibited the highest delay severity and variability.
- Several region–shipping routes experienced delay rates exceeding 70%.
- Delayed deliveries contributed significantly to revenue at risk.
- Pet Shop products showed the highest operational risk among departments.
- Bulk orders experienced slightly higher delays than single-item orders.
- Transfer payments were associated with elevated delay and cancellation rates.

---

## Key Visualizations

### Shipping Mode Performance Analysis

![Shipping Mode Analysis](images/shipping_mode_analysis.png)

### Regional Delivery Risk Analysis

![Regional Analysis](images/regional_delay_analysis.png)

### Revenue at Risk by Product Category

![Revenue Impact](images/revenue_at_risk.png)

### Route-Level Risk Analysis

![Route Analysis](images/route_risk_analysis.png)

### Customer Segment Performance

![Customer Analysis](images/customer_segment_analysis.png)

### Seasonal Delivery Trends

![Seasonal Trends](images/seasonal_trends.png)

---

## Tech Stack

| Tool | Usage |
|--------|--------|
| Python | Core Analysis |
| Pandas | Data Cleaning & Transformation |
| NumPy | Feature Engineering & Metrics |
| Matplotlib | Visualization |
| Seaborn | Statistical Plots & Heatmaps |
| Jupyter Notebook | Analysis Environment |

---

## Skills Demonstrated

### Data Analytics

- Exploratory Data Analysis (EDA)
- Data Cleaning
- Feature Engineering
- KPI Development
- Data Visualization
- Business Analytics

### Operational Analytics

- Supply Chain Analytics
- Logistics Performance Analysis
- Revenue Impact Assessment
- Process Optimization
- Risk Identification

### Business Intelligence

- Customer Segmentation
- Trend Analysis
- KPI Benchmarking
- Insight Generation
- Decision Support

### Technical Skills

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## Project Structure

```text
Supply-Chain-Performance-Analytics/

├── Supply_Chain_Performance_Analytics.ipynb
├── README.md
└── images/
    ├── shipping_mode_analysis.png
    ├── regional_delay_analysis.png
    ├── revenue_at_risk.png
    ├── route_risk_analysis.png
    ├── customer_segment_analysis.png
    └── seasonal_trends.png
```

---

## How to Run

```bash
git clone https://github.com/your-username/Supply-Chain-Performance-Analytics.git

cd Supply-Chain-Performance-Analytics

pip install pandas numpy matplotlib seaborn jupyter

jupyter notebook Supply_Chain_Performance_Analytics.ipynb
```

---

## Business Impact

This analysis demonstrates how data can be used to:

- Improve delivery performance
- Reduce operational inefficiencies
- Identify high-risk logistics routes
- Improve customer satisfaction
- Prioritize operational interventions
- Protect revenue through proactive monitoring

---

## Author

**Rithish Rao**  
BITS Pilani Hyderabad Campus  
Mechanical Engineering

Interested in Data Analytics, Business Analytics, Product Analytics, Operations Analytics, and Financial Analytics.
