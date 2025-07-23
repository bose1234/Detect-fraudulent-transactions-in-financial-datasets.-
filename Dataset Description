# Detect-fraudulent-transactions-in-financial-datasets.-
This project demonstrates how Splunk Enterprise can be used to detect fraudulent transactions in financial datasets. By analyzing transaction patterns, the project identifies high-risk categories, suspicious merchants, and trends over time.
#  Dataset Description.
The dataset consists of payment transactions from various customers over a four-month simulated period.

Key Columns:

Step: Transaction month (0 = May, 1 = June, 2 = July, 3 = August)

Customer: Customer ID

Age: Age group (0.0 = ≤18, 1.0 = 19-25, etc.)

Gender: F = Female, M = Male

Merchant: Merchant ID

Category: Transaction category

Amount: Purchase amount

Fraud: 1 = Fraudulent, 0 = Non-Fraudulent

------

 # Key Splunk Queries
 # 1. Fraud vs Non-Fraud Count

ini
Copy
Edit
index="fraud_detection_fresh" | stats count by fraud

# 2. Fraud by Category

ini
Copy
Edit
index="fraud_detection_fresh" fraud=1 | stats count by category

# 3. Fraud Trend by Month (Step)

ini
Copy
Edit
index="fraud_detection_fresh" fraud=1 | stats count by step

# 4. Top Merchants Involved in Fraud

bash
Copy
Edit
index="fraud_detection_fresh" fraud=1 | stats count by merchant | sort -count | head 5

# Key Findings
Highest Fraud Category: es_transportation (90.5% of fraud cases)

Peak Fraud Month: Step 2 (July)

Top Merchants: Identified 5 merchants with repeated fraud cases

# Tools Used
Splunk Enterprise – Log analysis & visualization

CSV Transaction Dataset – Prepared for Splunk ingestion

# Deliverables
Fraud Detection Report (PDF) – Detailed findings with charts

Splunk Dashboards & Visualizations – Screenshots included

👩‍💻 Author
Abosede Ogunlade – Cybersecurity Analyst | Digital Marketer


