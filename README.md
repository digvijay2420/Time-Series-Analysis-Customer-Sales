# Time-Series-Analysis-Customer-Sales
Time Series Analysis of retail shopping data using ARIMA and SARIMA models for forecasting customer sales patterns.
## 📌 Problem Statement
Retail businesses often struggle to accurately forecast customer demand and sales.  
This project applies **Time Series Analysis (TSA)** techniques to shopping transaction data to uncover trends, seasonality, and forecast future sales.  

---

## 🎯 Objectives
- Analyze customer shopping data using Time Series Analysis.  
- Identify patterns such as **trend, seasonality, and irregularities**.  
- Build predictive models (**ARIMA, SARIMA**) for sales forecasting.  
- Evaluate model accuracy using ADF, KPSS, AIC/BIC, and residual diagnostics.  
- Provide actionable insights for **retail optimization**.  

---

## 📂 Repository Structure
Time-Series-Analysis-Customer-Sales/
│── data/
│    └── DATASET_LINK.md                   # Google Drive link to full dataset
│
│── notebooks/
│    └── TSA_project.ipynb                 # Jupyter Notebook with code & outputs
│
│── docs/
│    └── TSA_project_report.pdf                   # (optional) Detailed report (PDF)
│
│── requirements.txt                       # Python dependencies
│── README.md                              # Project overview (this file)

---

## 📊 Dataset
- **Source**: Customer Shopping dataset.  
- **Focus**: Clothing category purchases using credit card.  
- **Size**: 7.19 MB (~500+ transactions).  
- **Variables**:  
  - `invoice_date` (timestamp)  
  - `category` -> Product type(Clothing,Shoes etc..)
  - `payment_method` -> Method of payment(Cash, Credit Card or Debit Card)
  - `price` -> Price of the product
  - `quantity`-> no of items purchased
  - `customer_id`-> ID of customer
  - `invoice_no`-> Unique number assigned to each transaction.
  - `gender`-> Gender of the customer(Male/Female)
  - `shopping_mall` → Name of the mall where purchase took place.

📂 **Access**  
 - Link: [Google Drive](https://drive.google.com/file/d/1xcnHH3ShArl7sml8kmDm3C_jKW-7A6Y9/view?usp=drive_link)

---


## 🔍 Methodology
1. **Data Preprocessing**  
   - Converted dates, handled missing values.  
   - Aggregated daily sales totals.  

2. **Exploratory Data Analysis (EDA)**  
   - Visualized trends, seasonality, and anomalies.  
   - Conducted decomposition of time series.  

3. **Stationarity Testing**  
   - Augmented Dickey-Fuller (ADF) test.  
   - KPSS test.  

4. **Modeling**  
   - Implemented ARIMA and SARIMA models.  
   - Selected parameters using ACF/PACF plots.  
   - Compared AIC/BIC values.  

5. **Forecasting**  
   - Generated daily revenue forecasts.  
   - Predicted total sales for **Jan 1, 2024** as a case study.  

---

## 📈 Results & Insights
- **ARIMA(5,1,0)** provided a good fit with stationary data.  
- **SARIMA** captured **weekly sales patterns** (higher weekends, lower weekdays).  
- Forecasting showed revenue patterns consistent with historical sales.  
- Key insight: Proper forecasting helps **reduce overstocking/stockouts** and align promotions with high-sales periods.  

---

## 🛠️ Tech Stack
- **Python**: `pandas`, `numpy`, `statsmodels`, `scipy`, `matplotlib`, `seaborn`, `plotly`  
- **Jupyter Notebook** for analysis & visualization  
- **PDF** for report documentation  

---

## 🚀 How to Run
```bash
git clone https://github.com/<digvijay2420>/Time-Series-Analysis-Customer-Sales.git
cd Time-Series-Analysis-Customer-Sales
pip install -r requirements.txt
jupyter notebook notebooks/TSA_project.ipynb

---

## 📝 Authors
- **Digvijay Singh**  

*(Project under STAT-545: Time Series Analysis, Pondicherry University, April 2025)*

