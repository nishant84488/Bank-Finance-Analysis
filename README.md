# 🏦 Power BI Bank Loan Portfolio Analysis: From SQL to Strategy

This project delivers a complete, end-to-end financial analysis of a bank's lending portfolio. It is anchored by a detailed methodology and culminates in a dynamic, interactive **Power BI Dashboard**.

The goal is to provide executive and risk management teams with clear, real-time insights to assess portfolio health, track growth, and proactively manage risk exposure.

---

## 📂 Project Repository Files

This repository contains both the documentation and the final presentation layer of the financial model.

| File Name                         | Description                            | Role in Project |
|----------------------------------|----------------------------------------|------------------|
| **`Bank Finance Project.docx`**  | The comprehensive project documentation. | Contains the **business requirements**, **data dictionary**, and all the **underlying SQL queries** (e.g., `SUM(loan_amount)`, `AVG(dti)`) used to calculate the dashboard metrics. |
| **`finance project final Dashbord.pbix`** | The final analytical output.         | The interactive **Power BI Dashboard file** containing all the visualizations, key performance indicators (KPIs), and detailed reports. |

---

## 📈 Key Performance Indicators (KPIs) & Metrics

The analysis is driven by robust SQL and DAX logic to calculate three critical categories of metrics.

### 1. Portfolio Volume & Growth

These metrics track the scale and momentum of lending operations, essential for performance review and forecasting.

- **Total Loan Applications:** Calculated using `COUNT(id)`  
- **Total Funded Amount:** The total capital deployed, calculated using `SUM(loan_amount)`  
- **Total Amount Received:** The bank's cash flow, calculated using `SUM(total_payment)`  
- **Trend Analysis:** All key metrics are tracked with **Month-to-Date (MTD)** and **Month-over-Month (MoM)** comparisons

### 2. Risk & Profitability Indicators

These are the quantitative measures of portfolio quality and return.

- **Average Interest Rate:** Weighted average return, `AVG(int_rate) * 100`  
- **Average Debt-to-Income (DTI) Ratio:** Core risk metric, `AVG(dti) * 100`

### 3. Risk Management: Good vs. Bad Loans

A central feature is the binary categorization of the loan book for instant risk assessment.

| Category      | Definition (based on `loan_status`)     | Key Metrics Tracked |
|---------------|------------------------------------------|----------------------|
| **Good Loans** | Loans that are 'Fully Paid' or 'Current' | Success Rate, Capital Preserved, Total Returns |
| **Bad Loans**  | Loans that have been 'Charged Off'       | Default Rate, Funded Amount Lost, Pre-Charge-Off Payments |

---

## 💻 Technical Architecture

This project integrates three tech layers to deliver a complete data analytics stack:

1. **Data Source Layer**: Raw data stored in `bank_loan_data` table in SQL DB  
2. **Transformation Layer (SQL / Power Query)**: SQL queries preprocess and shape the data for analysis  
3. **Presentation Layer (Power BI)**: Data is loaded into Power BI where all visualizations and interactions are built

---

## 🚀 Getting Started & Viewing the Dashboard

### Prerequisites

- **Power BI Desktop**: Required to open the `.pbix` file (Free from Microsoft)

### Instructions

1. Download or clone the repository  
2. Open `finance project final Dashbord.pbix` in Power BI Desktop  
3. Interact with slicers, filters, and dashboards to explore portfolio performance

---

## 🤝 Contribution

This project is a solid template for building financial dashboards. Contributions are welcome!

1. Fork the repository  
2. Create your Feature Branch (`git checkout -b feature/advanced-dax-model`)  
3. Commit your changes and open a Pull Request  

---
