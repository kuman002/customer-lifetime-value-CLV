# Customer Lifetime Value Prediction using Probabilistic Modeling

**Author:** Kumaresan K  
**Techniques:** BG/NBD, Gamma-Gamma, RFM Segmentation  
**Goal:** Predict future customer value and enable value-based marketing strategy  

---

## 📌 Project Overview

Understanding which customers drive future revenue is critical for effective marketing and retention strategy. This project applies probabilistic Customer Lifetime Value (CLV) modeling to transactional e-commerce data to estimate future purchasing behavior and monetary contribution at the individual customer level.

Using the **BG/NBD model** for purchase frequency and the **Gamma-Gamma model** for monetary value, we predict expected future revenue and segment customers into value tiers (Low, Mid, High, VIP).

The analysis demonstrates how raw transaction data can be transformed into forward-looking customer intelligence for strategic decision-making.

---

## 🎯 Objectives

- Model repeat purchasing behavior and customer survival probability
- Estimate future customer lifetime value (CLV)
- Identify high-value customer segments
- Analyze revenue concentration across segments
- Derive actionable marketing strategies

---

## 🗂 Dataset

Online Retail transactional dataset containing:

- Invoice date
- Quantity and price
- Customer ID
- Transaction revenue

Each row represents a product-level transaction.

---

## 🧮 Methodology

### 1. Data Preparation
- Removed invalid and anonymous transactions
- Filtered returns and negative quantities
- Computed transaction revenue
- Converted timestamps

### 2. Cohort Analysis
Customer retention evaluated by acquisition month cohorts to validate repeat purchase behavior and CLV modeling assumptions.

### 3. RFM Feature Engineering
Customer behavior summarized using:

- **Recency** — time between first and last purchase
- **Frequency** — repeat purchase count
- **Monetary** — average transaction value

### 4. BG/NBD Model
Estimated:

- Expected future purchase frequency
- Probability customer is still active

### 5. Gamma-Gamma Model
Estimated expected monetary value per future purchase.

### 6. CLV Estimation
Combined models to predict **6-month Customer Lifetime Value** for each customer.

### 7. CLV Segmentation
Customers segmented into quartiles:

- Low
- Mid
- High
- VIP

---

## 📊 Key Results

- Customer value is highly skewed with strong heterogeneity
- A small VIP segment drives the majority of predicted revenue
- Recent purchasing activity is the strongest predictor of future value
- Historical purchase volume alone does not indicate future profitability

Example insight:

> Customers with high historical frequency but long inactivity exhibit near-zero predicted CLV, while recently active customers show substantially higher future value.

---

## 📈 Visualizations

The project includes:

- Cohort retention heatmap
- RFM distributions
- BG/NBD frequency-recency matrix
- CLV distribution
- CLV segment comparison
- Revenue contribution by segment

---

## 💡 Marketing Strategy Implications

CLV segmentation enables value-based targeting:

- **VIP:** retention & loyalty programs
- **High:** upsell and cross-sell
- **Mid:** engagement nurturing
- **Low:** cost-efficient reactivation

Revenue concentration analysis confirms that prioritizing high-value segments maximizes marketing ROI.

---

## 🧰 Tech Stack

- Python
- Pandas / NumPy
- Matplotlib / Seaborn
- Lifetimes (BG/NBD & Gamma-Gamma)
- Jupyter Notebook

---

## 📁 Repository Structure

```text
CLV Prediction/
│
├── notebook/
│   └── CLV_analysis.ipynb
│
├── data/
│   ├── raw/
│   │   └── data.csv
│   └── cleaned/
│       └── cleaned_data.csv
│
├── images/
│
├── requirements.txt.txt
└── README.md
```

---

## ▶️ How to Run

```bash
pip install -r requirements.txt.txt
```

Open notebook:

```text
notebook/CLV_analysis.ipynb
```

---

## 📚 Business Value

This project demonstrates how probabilistic data science models can:

- Forecast customer revenue
- Identify high-value customers
- Optimize marketing allocation
- Support retention strategy

---

## 👤 Author

**Kumaresan K**  
Data Science | Machine Learning | Customer Analytics

- LinkedIn: [https://www.linkedin.com/in/kumaresan-k-4289452b4](https://www.linkedin.com/in/kumaresan-k-4289452b4)
- GitHub: [https://github.com/kuman002](https://github.com/kuman002)

---

## ⭐ Key Skills Demonstrated

- Probabilistic modeling
- Customer lifetime value analytics
- Behavioral segmentation
- Marketing data science
- Business insight generation
