BankGuard — Mzantsi
Team: Siziphiwe Nkweba, Akona Majongile & Sumaya Khan Client: MzansiBank

Tech Stack
Languages & Libraries: Python, NumPy, Pandas, Matplotlib
Environment: Jupyter Notebook
Data: CSV (also supports API / SQL acquisition)
Collaboration: Git, GitHub
The project covers the full data lifecycle: acquisition from CSV/API/SQL, NumPy and Pandas, inspection, cleaning, datetime handling, duplicates/outliers, merging, grouping, feature engineering, scaling, encoding, pipelines, reshaping, visualisation and exporting.

Problem Statement
MzansiBank has provided customer and transaction data and requires the data science team to deliver a reproducible analysis solution. The key challenges are:

Customer usage — Understand how customers interact with the bank and its services.
Transaction concentration — Identify where transaction activity is most frequent or clustered.
Financial risk — Detect transactions that may indicate potential fraud or financial risk.
Executive reporting — Present clear, actionable insights to the bank's leadership team.
Pipeline Overview
1. Loading Trusted Datasets
Datasets were securely saved onto local machines.
Python was used to import each dataset systematically.
This ensured each dataset was ready for the data-cleaning stage.
2. Data Validation & Cleaning
A structured transformation and cleaning process was applied consistently across all datasets:

Filling in missing values
Removing duplicate records
Assigning the correct data types to each feature
Standardising date formats and string values for cohesion
3. Integration
The transactions, accounts, and customers datasets were merged. This integration was necessary because features from all three sources were required to answer the key business questions — and it was only possible once all datasets were cohesive and clean.

4. Feature Engineering
Features added during this phase include:

Feature	Purpose
customer_average_transaction	Baseline spend per customer
high_value_transactions	Flag for unusually large transactions
transaction_days	Day-of-week activity
Date features: year & month	Time-based trend analysis
customer_transaction_count	Activity volume per customer
customer_total_transaction_value	Lifetime value per customer
customer_max_transaction	Peak spend per customer
Transaction Analytics
Which transaction type is most common?
Transaction Type	No. of Transactions
Refund	50,000
Withdrawal	100,000
Deposit	100,000
Payment	150,000
Transfer	180,000
Purchase	410,000
Purchase is by far the most common transaction type.

Which channels are most frequently used?
Channel	Percentage
Online	43.5%
Mobile	31.9%
POS	24.6%
Online is the dominant transaction channel.

What are the busiest transaction days?
Day	No. of Transactions
Monday	145,300
Tuesday	142,350
Wednesday	143,200
Thursday	142,600
Friday	143,450
Saturday	141,300
Sunday	141,600
Monday is the busiest transaction day, though volumes are fairly even across the week.

How does transaction behaviour change over time?
Year	No. of Transactions
2025	630,000
2026	370,000
Transaction behaviour decreased significantly from 2025 to 2026.

Which province generates the most transaction value?
Province	Transaction Value
Gauteng	21,000
KwaZulu-Natal	14,250
Western Cape	8,600
Eastern Cape	7,100
Limpopo	5,700
Free State	4,300
Mpumalanga	4,250
North West	3,600
Northern Cape	2,150
Customer Analytics
Total customers: 99,903
Which province has the most customers?
Province	No. of Customers
Gauteng	30,000
KwaZulu-Natal	20,000
Western Cape	12,000
Eastern Cape	10,000
Limpopo	8,000
Free State	6,000
Mpumalanga	6,000
North West	5,000
Northern Cape	3,000
Which account type is most popular?
Account Type	No. of Customers
Savings	40,500
Cheque	39,000
Credit	11,500
Which age group has the highest average income?
Age Group	Average Income
36–45	30,000
26–35	24,500
46–55	20,500
18–25	15,000
56–65	8,000
65+	2,000
Which customer segments generate the highest transaction value?
Customer Segment	Total Transaction Value ($)
Middle Income	4.4B
High Income	1.6B
Low Income	0.8B
Very High Income	0.4B
Business Intelligence & Risk
What percentage of transactions are labelled fraudulent?
0.64% of transactions are labelled fraudulent.

How many transactions are potentially suspicious?
Risk Rating	Number of Transactions
High	2,088
Unknown	18
Critical	17
Distribution of fraudulent transactions by channel
Channel	Percentage
Online	40.8%
Mobile	16.8%
POS	12.4%
App	11.5%
ATM	11.2%
Branch	6.0%
Unknown (NaN)	1.2%
The Online channel carries the largest share of fraudulent transactions (40.8%), mirroring its dominance in overall volume.

Which transaction type has the highest fraud rate?
Transaction Type	Fraud Count
Purchase	2,424
Transfer	1,415
Payment	1,153
Withdrawal	561
Deposit	548
Refund	298
Which merchants are associated with the highest risk?
Merchant Category	High-Risk Transactions
Healthcare	232
Grocery	223
Fuel	220
Clothing	214
Restaurant	210
Other	205
Electronics	202
Entertainment	202
Online Services	193
Travel	189
High-risk transactions are evenly spread across merchant categories — no single category dominates.

Which provinces have the highest risk?
Province	High-Risk Transactions
Limpopo	258
North West	257
KwaZulu-Natal	256
Western Cape	247
Gauteng	222
Eastern Cape	220
Free State	220
Mpumalanga	215
Northern Cape	210
High-risk transactions are broadly distributed across all provinces, with Limpopo, North West and KwaZulu-Natal marginally highest. Notably, Gauteng — the largest province by customers and value — does not have the most high-risk transactions.

Key Findings
Most common transaction type: Purchase
Most common transaction channel: Online
Busiest transaction day: Monday
Highest transaction value province: Gauteng
Transaction behaviour significantly decreased from 2025 to 2026
0.64% of transactions are fraudulent; ~2,100+ are rated High/Critical risk
Fraud is concentrated in the Online channel (40.8%) but spread evenly across merchants and provinces
Recommendations
Transaction Recommendations
Enhance purchase services — Purchases are the most common transaction type; invest in seamless payment solutions, loyalty programs, and merchant partnerships to strengthen this core activity.
Optimize the online channel — With online dominant, improve digital platforms (mobile app, website) for speed, security, and user experience; expand digital customer support.
Leverage the Monday peak — Use targeted promotions, system capacity planning, and fraud monitoring on Mondays to manage high volumes effectively.
Focus on Gauteng — As the highest-value province, prioritize marketing campaigns, branch services, and tailored financial products there.
Address declining activity — Investigate the 2025–2026 drop in transaction behaviour via customer re-engagement strategies, product innovation, and competitive benchmarking.
Customer Recommendations


Grow the under-35 base — The 36–45 group earns the most today, but the 26–35 segment is the growth engine; target them with savings and credit products that mature with their income.
Deepen Savings engagement — Savings is the most popular account type (40,500 customers); cross-sell Cheque and Credit products to this base.
Prioritize the Middle Income segment — It generates the highest total transaction value ($4.4B); design tailored bundles, rewards, and retention programs for it.
Regional expansion beyond Gauteng — Gauteng leads in customers (30,000), but KwaZulu-Natal and Western Cape show strong secondary bases worth targeted acquisition campaigns.
Business Intelligence & Risk Recommendations


Harden the Online channel — It accounts for 40.8% of fraudulent transactions; deploy stronger authentication (2FA/biometrics), real-time fraud scoring, and step-up verification for online payments.
Investigate High & Critical risk transactions first — Triage the ~2,100 High/Critical-rated transactions immediately; they represent the most probable active fraud.
Monitor Transfers and Payments — After Purchases, these types carry the highest fraud counts; apply velocity checks and amount-threshold alerts.
Province-agnostic monitoring — High-risk activity is evenly distributed across provinces, so fraud controls should be national rather than regionally concentrated.
Close data gaps — 1.2% of fraudulent transactions have unknown (NaN) channels and 18 have unknown risk ratings; enforce complete data capture at the point of transaction.