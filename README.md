# 💼 Banking – Loan Risk & Profitability Dashboard (Excel)

An Excel-based project analyzing consumer lending data to identify risk patterns, predict defaults, and measure profitability using interactive dashboards and advanced Excel formulas.

---

## 📌 Objectives

- Predict likelihood of default using loan amount, income, and employment length.
- Calculate Loan Profitability Index (LPI) and Risk-Adjusted Return (RAR).
- Visualize trends in interest rates, default risks, and loan conditions.
- Enable dynamic analysis via PivotTables, slicers, and charts.

---

## 📊 Tools & Techniques

- **Software**: Microsoft Excel
- **Functions**: `SUMPRODUCT`, `SUMIF`, `IF`, `MODE`, `MATCH`, `GETPIVOTDATA`
- **Visuals**: Pivot Charts, Risk Matrix, Donut, Scatter, Slicers
- **Data**: `loan_final313_.csv`

---

## 🔍 Key Metrics

- **LPI**  
  `=IF(loan_condition="Bad Loan", interest_rate*(term/12)*0.0505, interest_rate*(term/12))`

- **RAR**  
  `= interest_rate * (1 - (Bad Loans / Total Loans))`

- **Default Score**  
  `= 0.5*Norm_Loan_Amount - 0.3*Norm_Income - 0.2*Norm_Emplen`

- **Weighted Avg. Interest Rate**  
  `= SUMPRODUCT(...) / SUMIF(...)` per income category

---

## 💡 Key Insights

- Lower-income borrowers face higher interest rates.
- Grades C–E are moderately risky but yield better returns.
- Recovery from bad loans is just **5.05%**, emphasizing risk management.
- Risk-adjusted returns increase with grade but carry higher default likelihood.

---

## 📁 Files

- `loan_final313_.csv` – Source dataset  
- `Loan_Analysis_Dashboard.xlsx` – Final dashboard  
- `/Screenshots/` – Visual evidence and charts

---

## 👤 Author

**Naveen Kakarla** – Data Analyst | Excel Enthusiast

---

## 🏷️ Tags

`#Excel` `#LoanAnalysis` `#BankingDashboard` `#RiskProfiling` `#DataVisualization` `#RAR` `#LPI`

