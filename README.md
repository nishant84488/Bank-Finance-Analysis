# Bank-Finance-Analysis



\# 🏦 Power BI Bank Loan Portfolio Analysis: From SQL to Strategy



This project delivers a complete, end-to-end financial analysis of a bank's lending portfolio. It is anchored by a detailed methodology and culminates in a dynamic, interactive \*\*Power BI Dashboard\*\*.



The goal is to provide executive and risk management teams with clear, real-time insights to assess portfolio health, track growth, and proactively manage risk exposure.



---



\## 📂 Project Repository Files



This repository contains both the documentation and the final presentation layer of the financial model.



| File Name | Description | Role in Project |

| :--- | :--- | :--- |

| \*\*`Bank Finance Project.docx`\*\* | The comprehensive project documentation. | Contains the \*\*business requirements\*\*, \*\*data dictionary\*\*, and all the \*\*underlying SQL queries\*\* (e.g., `SUM(loan\_amount)`, `AVG(dti)`) used to calculate the dashboard metrics. |

| \*\*`finance project final Dashbord.pbix`\*\* | The final analytical output. | The interactive \*\*Power BI Dashboard file\*\* containing all the visualizations, key performance indicators (KPIs), and detailed reports. |



---



\## 📈 Key Performance Indicators (KPIs) \& Metrics



The analysis is driven by robust SQL and DAX logic to calculate three critical categories of metrics.



\### 1. Portfolio Volume \& Growth

These metrics track the scale and momentum of lending operations, essential for performance review and forecasting.



\* \*\*Total Loan Applications:\*\* Calculated using `COUNT(id)`.

\* \*\*Total Funded Amount:\*\* The total capital deployed, calculated using `SUM(loan\_amount)`.

\* \*\*Total Amount Received:\*\* The bank's cash flow, calculated using `SUM(total\_payment)`.

\* \*\*Trend Analysis:\*\* All key metrics are tracked with \*\*Month-to-Date (MTD)\*\* and \*\*Month-over-Month (MoM)\*\* comparisons for immediate identification of growth or decline trends.



\### 2. Risk \& Profitability Indicators

These are the quantitative measures of portfolio quality and return.



\* \*\*Average Interest Rate:\*\* The weighted average return on the loans, calculated using `AVG(int\_rate) \* 100`.

\* \*\*Average Debt-to-Income (DTI) Ratio:\*\* A core risk metric, calculated using `AVG(dti) \* 100` to gauge the borrower's financial stress.



\### 3. Risk Management: Good vs. Bad Loans

A central feature is the binary categorization of the loan book for instant risk assessment.



| Category | Definition (based on `loan\_status`) | Key Metrics Tracked |

| :--- | :--- | :--- |

| \*\*Good Loans\*\* | Loans that are 'Fully Paid' or 'Current'. | Success Rate (%), Total Capital Preserved, Total Returns Generated. |

| \*\*Bad Loans\*\* | Loans that have been 'Charged Off'. | Default Rate (%), Total Funded Amount lost, Payments Received before Charge-Off. |



---



\## 💻 Technical Architecture



The project seamlessly integrates three layers of technology to create the final dashboard:



1\.  \*\*Data Source Layer:\*\* The raw data resides in a relational database table (assumed to be named `bank\_loan\_data`).

2\.  \*\*Transformation Layer (SQL/Power Query):\*\* The \*\*SQL queries\*\* outlined in the project's documentation are the brain of the analysis. They define how raw data is aggregated, categorized, and prepared for visualization.

3\.  \*\*Presentation Layer (Power BI):\*\* The pre-calculated data is imported and modeled within the \*\*`.pbix` file\*\*, where interactive charts, slicers, and scorecards are created to bring the financial story to life.



\## 🚀 Getting Started \& Viewing the Dashboard



No complex installation or environment setup is required to interact with the final output.



\### Prerequisites

\* \*\*Power BI Desktop:\*\* Required to open and view the `.pbix` file. (Available as a free download from Microsoft).



\### Instructions

1\.  Download or clone the repository.

2\.  Open the file \*\*`finance project final Dashbord.pbix`\*\* using Power BI Desktop.

3\.  The dashboard will load, allowing you to filter by status, time period, and other dimensions to explore the portfolio's performance.



---



\## 🤝 Contribution



This project is a strong template for financial data analysis. If you have suggestions for new risk models, efficiency improvements in the SQL, or enhanced DAX measures, your contributions are highly welcome!



1\.  Fork the repository.

2\.  Create your Feature Branch (`git checkout -b feature/advanced-dax-model`).

3\.  Commit your changes and open a Pull Request.



