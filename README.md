# Bank Transactions Analysis Dashboard

## 📌 Project Overview
This project delivers an interactive **Power BI dashboard** analyzing bank transactions to uncover trends, transaction patterns, and account behaviors.  
The solution covers the full BI workflow — **data import, cleaning, transformation (Power Query M code), and dashboard creation**.

---

## 🛠 Tools & Technologies
- **Power BI** – Data visualization & dashboarding  
- **Power Query (M Language)** – Data extraction, transformation & cleaning  
- **CSV Data Source** – Raw transactional records  

---

## 📊 Key Features
- Transaction trend analysis over time  
- Segmentation by transaction type  
- Monthly and yearly transaction summaries  
- Balance monitoring and patterns identification  

---

## 🔄 Workflow
1. **Data Ingestion** – Imported raw `bank transaction_data.csv` into Power BI.  
2. **Data Transformation** – Used **Power Query M code** to:
   - Remove blanks & inconsistencies  
   - Format dates and numeric fields  
   - Create calculated columns for **Credit Type** ,**Year** and **Month**  
3. **Data Visualization** – Developed an interactive dashboard with:
   - Monthly trends
   - Transaction type breakdown
   - Yearly summaries  

---
## 1. Dataset Summary
- **Total transactions:** `1,000`
- **Total transaction value:** `$771,165.29`
- **Average transaction value:** `$771.17`

---

## 2. Transaction Status Overview
| Status   | Count | Value ($)   | % of Total Transactions |
|----------|-------|-------------|-------------------------|
| Failed   | 513   | 386,422.38  | 50.1%                   |
| Success  | 487   | 384,742.91  | 49.9%                   |

**Insight:**  
The failure rate is **50%**, which is significantly higher than industry norms.  
This could be due to:
- Strong fraud prevention systems blocking suspicious transactions
- Operational or system-related issues

---

## 3. Transaction Type Breakdown
| Type       | Count | Total Amount ($) |
|------------|-------|------------------|
| Deposit    | 316   | 252,042.62       |
| Transfer   | 374   | 291,776.55       |
| Withdrawal | 310   | 227,346.12       |

**Insight:**  
- **Transfers** account for the highest total value (~38% of total funds moved).  
- Deposits and withdrawals are close in both count and total value.

---

## 4. Fraud Analysis
- **Fraudulent transactions:** `481` (48.1% of all transactions)
- **Fraudulent transaction value:** `$378,863.90` (49.13% of total funds moved)

### Fraud by Transaction Type:
| Type       | Fraud Count | Fraud Amount ($) |
|------------|-------------|------------------|
| Deposit    | 167         | 130,061.30       |
| Transfer   | 170         | 135,385.93       |
| Withdrawal | 144         | 113,416.67       |

**Insight:**  
- Fraud is **spread evenly** across all transaction types.  
- The nearly 50% fraud rate is far above acceptable banking thresholds (<1% in most institutions).  
- This points to **systemic vulnerabilities** rather than isolated weaknesses.

---

## 5. Key Red Flags
1. **Extremely high fraud rate** (48.1%).
2. **50% failure rate** in transactions.
3. Fraud is **not isolated** to one type — systemic issues likely exist.
4. High-value transfers are a **prime fraud target**.

---

## 6. Recommendations
- **Immediate security audit**: Strengthen authentication, device validation, and transaction monitoring.
- **Behavioral analytics**: Detect abnormal transaction patterns (location, frequency, amount).
- **Separate analysis** of failed vs. successful fraud attempts to measure control effectiveness.
- **Enhanced monitoring** on transfers due to high monetary impact.


