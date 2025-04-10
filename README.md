# My-project
Market Basket Analysis
This project applies Market Basket Analysis on a retail transaction dataset using the Apriori algorithm for association rule mining. The analysis helps uncover hidden patterns in customer purchasing behavior, aiding in product placement strategies, recommendations, and boosting sales.

🧾 Dataset
File Name: Ck dataset (1).csv
Description: This dataset contains transaction records where each row represents a product purchase within a single transaction (or invoice). It includes:

InvoiceNo
StockCode
Description
Quantity
InvoiceDate
UnitPrice
CustomerID
Country

📊 Objective
To analyze customer purchasing behavior and generate association rules that identify frequent product combinations using:
Data preprocessing
Transaction grouping
Apriori algorithm
Rule filtering based on support, confidence, and lift

🛠️ Tools & Libraries
Python
Pandas
Matplotlib / Seaborn
mlxtend (for Apriori and association_rules)

🔍 Key Steps
1. Data Cleaning
    Removed null and duplicate values
    Filtered relevant transactions (e.g., excluding refunds or negative quantities)
2. Transaction Conversion
    Grouped transactions by InvoiceNo
    Transformed into a binary matrix (one-hot encoding style) for the Apriori algorithm
3. Frequent Itemset Mining
    Used mlxtend’s Apriori implementation
    Set a minimum support threshold
4. Association Rule Generation
    Extracted rules based on support, confidence, and lift
    Focused on actionable insights (e.g., rules with high lift)
5. Visualization
    Bar plots of most frequent itemsets
    Scatter plots for rule evaluation

