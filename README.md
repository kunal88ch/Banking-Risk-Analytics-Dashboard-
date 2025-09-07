# 🏦 Banking Risk Analytics Dashboard (Power BI)

## 📌 Project Overview
The **Banking Risk Analytics Dashboard** is a Power BI project designed to help financial institutions minimize lending risks by analyzing client profiles, deposits, loans, and engagement metrics. By leveraging interactive dashboards and KPIs, banks can make smarter decisions on whether to approve or reject loan applications.

---

## 🎯 Problem Statement
Banks face a major challenge in assessing the **risk of loan defaults**. Without proper analytics, they risk losing money when lending to customers. This project provides a **data-driven solution** to evaluate clients based on their financial behavior and profiles.

---

## ✅ Solution
Using **Power BI dashboards**, this project enables:
- Loan approval decisions based on applicant profiles.  
- Risk analysis through deposits, credit card balances, and loans.  
- Tracking client engagement with banks over time.  

---

## 📂 Dataset
The dataset contains multiple interlinked tables such as:
- **Banking Relationship**  
- **Client-Banking**  
- **Gender**  
- **Investment Advisor**  
- **Period**  

---

## 🔧 Data Cleaning & Transformation
Key transformations include:
- **Engagement Timeframe**: Timeline of client relationships with banks.  
- **Engagement Days**: Days since the client joined the bank.  
- **Income Bands**: Categorized income into Low (<100K) and Mid (<300K).  
- **Processing Fees**: Derived from Fee Structure (e.g., 0.05 for high fee structure).  

---

## 📊 Key DAX Measures
- **Total Clients** = `DISTINCTCOUNT('Clients - Banking'[Client ID])`  
- **Total Loan** = `[Bank Loan] + [Business Lending] + [Credit Cards Balance]`  
- **Engagement Days** = `DATEDIFF('Clients - Banking'[Joined Bank], TODAY(), DAY)`  
- **Total Fees** = `SUMX('Clients - Banking', [Total Loan] * 'Clients - Banking'[Processing Fees])`  

---

## 📌 KPIs
- Total Clients  
- Total Loan  
- Bank Loan  
- Business Lending  
- Total Deposits  
- Total Fees  
- Credit Card Balances  
- Engagement Length  

---

## 📈 Dashboards & Visuals
- **Home Dashboard**: Overview of all banking metrics.  
- **Loan Analysis Dashboard**: Loan distribution and repayment risk.  
- **Deposit Analysis Dashboard**: Deposits across different account types.  
- **Summary Dashboard**: High-level KPIs and insights.  

*(Add screenshots of your dashboards here for better visualization.)*  

---

## 🔎 Key Insights
- Private banks have a higher number of clients compared to public banks.  
- Income bands influence loan repayment capabilities.  
- Engagement length helps predict customer loyalty.  
- Insights on which nationality holds the highest loans.  

---

## 📌 Conclusion
The **Banking Risk Analytics Dashboard** empowers banks to **reduce financial risk** by providing clear insights into client behavior, loans, deposits, and engagement. It improves decision-making for loan approvals and strengthens overall risk management.

---

## 🚀 Future Work
- Predictive modeling for loan default risks.  
- Integration with real-time banking systems.  
- Advanced segmentation of clients for personalized offers.  
