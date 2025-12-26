# 🏦 Banking Risk Analytics Dashboard

## 📌 Project Overview
Banks face significant financial risk when lending to customers who may default. This project focuses on **banking risk analytics**, combining **Python-based exploratory data analysis (EDA)** with an **interactive Power BI dashboard** to help stakeholders assess credit risk, exposure concentration, and liquidity imbalance *before* approving or expanding loans.


---

## 🎯 Business Problem
Poor credit risk assessment can lead to:
- High non-performing assets (NPAs)
- Liquidity stress due to loan–deposit imbalance
- Excessive exposure to high-risk client segments

**Project Objective:**  
To analyze customer, loan, and deposit data to:
- Evaluate repayment likelihood
- Identify high-risk exposure
- Improve portfolio stability and lending decisions

---

## 🗂️ Dataset Overview
The dataset contains historical banking data with:
- Client demographics (Gender, Nationality, Income Band)
- Banking relationships (Retail, Private Bank, Commercial, Institutional)
- Loan details (Loan Amount, Business Lending, Credit Card Balance)
- Deposit details (Savings, Checking, Foreign Currency, Total Deposits)
- Risk indicators (Risk Score: High / Medium / Low)
- Engagement timeframe (Years with bank)

---

## 🧪 Exploratory Data Analysis (Python)
EDA is performed using **Python (Pandas, Matplotlib, Seaborn)**.

### Key EDA Steps
- Data cleaning and type corrections
- Handling missing and inconsistent values
- Feature engineering (Client Count, Loan-to-Deposit Ratio, Risk-Scores)
- Distribution and outlier analysis
- Risk segmentation by income band, tenure, and relationship type

### Key EDA Findings/Insights 

**Financial Behavior**: Customers who maintain checking accounts are likely to have savings accounts and vice versa. This suggests that individuals who engage more with banking services tend to manage their finances through multiple accounts.

**Marketing Opportunities**: If there’s a strong correlation, it presents an opportunity for targeted marketing campaigns. For example, we could promote savings account products to checking account holders to encourage them to save more.

**Risk Assessment**: High correlation points to lower risk profiles for customers with both types of accounts. These customers might be more financially stable and responsible, making them more desirable for loans or credit products.

**Customer Segmentation**: we can use this insight to segment customers based on their account types, allowing for tailored services and communication.

**Behavioral Patterns**: It indicate that customers are using checking accounts for daily transactions while saving in savings accounts, highlighting different financial behaviors. 

- Loan and deposit values are right-skewed, indicating concentration risk
- High-risk clients have disproportionately higher loan exposure
- Longer engagement does not always correlate with lower risk  

<p align="center">
  <img src="Images/EDA.png" width="800">
</p>


---

## 📊 Power BI Dashboard Structure
The dashboard is divided into **four analytical pages**, each answering a specific business question.

### 1️⃣ Executive Summary
**Purpose:** High-level portfolio health snapshot 
## 📊 Dashboard Preview

<p align="center">
  <img src="Images/Executive Summary.png" width="800">
</p>


**Key KPIs:**
- Total Clients: **3000**
- High Risk %: **32.8%**
- Total Loan Portfolio: **₹4.38bn**
- Loan-to-Deposit Ratio (LDR): **116%**

**Insights:**
- LDR above 100% indicates liquidity risk
- Significant concentration in high-risk clients

---

### 2️⃣ Loan Analysis
**Purpose:** Analyze loan exposure and concentration 
<p align="center">
  <img src="Images/Loan Analysis.png" width="800">
</p>

**Insights:**
- Business lending dominates total loan exposure (₹2.6bn)
- Private Banking shows higher high-risk loan concentration
- Loan exposure varies significantly by nationality and income band

---

### 3️⃣ Deposit Analysis
**Purpose:** Evaluate funding stability and deposit composition
<p align="center">
  <img src="Images/Deposit Analysis.png" width="800">
</p>
**Insights:**
- Total Deposits: **₹3.77bn**
- Savings and Checking accounts form the bulk of deposits
- European clients contribute higher deposits with lower default risk
- LDR target benchmark: **0.80** (current: **1.16**)

---

### 4️⃣ Summary & Risk Segmentation
**Purpose:** Combine risk, exposure, and actionability
<p align="center">
  <img src="Images/Summary.png" width="800">
</p>
**Key Visuals:**
- Client Segmentation Scatter Plot (Deposits vs Loans)
- Risk category table with conditional formatting
- Insights & Recommendations panel

**Scatter Plot Insight:**
- High-risk clients cluster in high-loan / low-deposit quadrant
- Low-risk clients show stronger deposit backing

---

## 🔍 Key Insights
- **Liquidity Risk:** Loan-to-Deposit Ratio at **116%** indicates overleveraging
- **Risk Concentration:** 32.8% of clients (984) classified as High Risk
- **Exposure Risk:** High-risk exposure totals **₹1.78bn**
- **Segment Opportunity:**
  - Private Banking clients contribute ~45% of deposits but only ~28% of loans
- **Low-Risk Growth Segment:** European clients show lowest default rates (~4.2%)

---

## ✅ Business Recommendations

### Immediate Actions
- Slow loan growth until LDR falls below 100%
- Increase deposit mobilization via long-term savings products

### Risk Mitigation
- Tighten credit approval for High Risk clients
- Apply stricter pricing and collateral requirements

### Growth Strategy
- Expand lending cautiously in Private Banking segment
- Target European and Low Risk clients for portfolio growth

### Monitoring & Governance
- Track High Risk % monthly
- Set early-warning thresholds for LDR breaches
- Use client segmentation scatter for pre-approval screening

---

## 🛠️ Tools & Technologies Used:
- **Python:** Pandas, Matplotlib & Seaborn
- **Power BI:** DAX, conditional formatting, drill-through, scatter analysis
- **SQL:** Data Ingestion, validation & aggregation

---

## 📌 Conclusion
This project demonstrates how combining **Python EDA** with **Power BI dashboards** can transform raw banking data into actionable risk insights. The solution supports proactive risk management, reduces default probability, and balances portfolio growth with liquidity stability.



