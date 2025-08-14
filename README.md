# 🏦 Bank Loan Summary Dashboard

<img width="1334" height="766" alt="Screenshot 1" src="https://github.com/user-attachments/assets/a214fa1a-9b69-4e48-a094-91bb37268002" />

## 📌 Project Overview
This project delivers a **comprehensive analysis of bank loan performance** using data from PostgreSQL and interactive dashboards in Power BI. It uncovers key lending patterns, repayment behavior, and customer profiles to support **better risk assessment, targeted marketing, and lending strategy optimization**.

The dataset contains **38,576 loan records** with details like loan status, funded amounts, repayment amounts, interest rates, debt-to-income ratio, customer demographics, and loan purposes.

---

## 📊 Key Visualizations
- **Summary Metrics Cards**  
  - **Total Loan Applications**: 39K  
  - **Total Amount Funded**: $436M  
  - **Total Amount Received**: $473M  
  - **Average Interest Rate**: 12%  
  - **Average DTI**: 13.3%  

- **Good Loan vs Bad Loan**  
  Donut chart showing **86.18% good loans** vs **13.82% bad loans**.

- **Loan Applications by Home Ownership**  
  Majority from **RENT** and **MORTGAGE** categories.

- **Trend Analysis**
  - Monthly applications (steady growth, peak in Dec).
  - State-level map (California leads in applications).
  - Loan term breakdown (73% are 36-month loans).

- **Demographic Insights**  
  Applications by employee experience and loan purpose — **Debt Consolidation** dominates.

- **Financial Health**  
  Funding vs repayment comparisons for each loan status.

---

## 🔍 Insights & Analysis
- **Healthy repayment behavior**: Over **86% of loans** are fully paid or current.
- **Debt consolidation loans** dominate, suggesting opportunities for bundled financial products.
- **Shorter loan terms (36 months)** are preferred, indicating a customer preference for faster payoff.
- **California** stands out as the highest loan application state — potential for targeted campaigns.
- Funding and repayment patterns show a strong recovery rate across most loan categories.

---

## 🛠 Technologies Used
- **Database**: PostgreSQL  
- **Query Tool**: pgAdmin 4  
- **Visualization**: Power BI (DAX measures, interactive filters, maps, trend charts)  
- **Languages**: SQL, DAX  
- **Data Source**: Loan dataset from internal banking database  

---

## 🚀 Project Steps
1. **Data Extraction**
   - Connected to PostgreSQL database (`Bankdb`) via pgAdmin 4.
   - Executed:
     ```sql
     SELECT * FROM loan;
     ```
2. **Data Cleaning**
   - Removed duplicates, fixed date formats, standardized numeric values.

3. **Data Loading**
   - Imported PostgreSQL data into Power BI using a direct connection.

4. **DAX Measures Creation**
   - Total Amount Funded  
   - Total Amount Received  
   - Average Interest Rate  
   - Average DTI  
   - Good Loan % and Bad Loan %

5. **Dashboard Building**
   - Designed two main dashboards:
     - **Performance Summary**
     - **Detailed Loan Insights**
   - Added slicers for loan purpose and grade filtering.

6. **Validation**
   - Cross-checked Power BI outputs with PostgreSQL aggregates.

---

## 📂 How to Use
- Clone this repository.  
- Open `.pbix` file in Power BI Desktop.  
- Use slicers to filter by loan purpose or grade.  
- Explore charts and hover for deeper insights.  
- Export results as needed.

---

## 📬 Contact  
👤 **Chaitanya Panicker**  
📧 chaitanya.panicker98@gmail.com  
🌐 https://www.linkedin.com/in/chaitanyapanicker 

---

## 📜 License  
This project is licensed under the **MIT License** — free to use, modify, and share with attribution.
