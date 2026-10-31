# 🛍️ Customer Shopping Behavior Analysis

End-to-end analysis of 3,900 retail purchases using Python, MS SQL Server and Power BI to uncover spending patterns, customer segments, product preferences and subscription behavior.

📚 Learning project. Built while following the tutorial by Amlan Mohanty. Original creator's GitHub: github.com/amlanmohanty1

# 📌 Project Overview
The goal is to guide business decisions by answering questions about revenue, discounts, shipping, subscriptions, loyalty and product performance.

# 📊 Dataset Summary
Rows: 3,900 | Columns: 18
Demographics: Age, Gender, Location, Subscription Status
Purchase details: Item Purchased, Category, Purchase Amount, Season, Size, Color
Behavior: Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type
Missing data: 37 values in Review Rating

# 🔧 Workflow
Python (pandas): loading, df.info() / .describe(), missing Review Rating values filled with the median rating per category, columns renamed to snake_case, created age_group and purchase_frequency_days, dropped redundant promo_code_used, loaded cleaned data into MSSQL.
SQL (MSSQL): 10 business questions (see below).
Power BI: interactive "Customer Behavior Dashboard".

# ❓ SQL Business Questions
#	Question	Key finding
1	Revenue by gender	Male 157,890 vs Female 75,191
2	Discount users spending above average	11 customers shown in report extract
3	Top 5 products by rating	Gloves (3.86), Sandals, Boots, Hat, Handbag
4	Standard vs Express shipping	Avg 58 vs 60
5	Subscribers vs non-subscribers	Same avg spend (59); non-subscribers 170,436 vs subscribers 62,645 total revenue
6	Most discount-dependent products	Hat (50%), Coat, Sneakers, Sweater, Pants
7	Customer segmentation	Loyal 3,116 · Returning 701 · New 83
8	Top 3 products per category	e.g. Jewelry, Blouse, Sandals, Jacket lead their categories
9	Repeat buyers & subscription	2,518 non-subscribed vs 958 subscribed
10	Revenue by age group	Young Adult 62,143 highest; Senior 55,763 lowest

# 📈 Dashboard

Dashboard Preview

KPIs: 3.9K customers · $59.76 average purchase · 3.75 average rating. Slicers: subscription, gender, category, shipping type.

# 💡 Business Recommendations
Boost subscriptions with exclusive benefits
Loyalty programs to convert repeat buyers into "Loyal"
Review discount policy to balance sales and margin
Product positioning around top-rated and best-selling items
Targeted marketing at high-revenue age groups and express-shipping users

# 🛠️ Tools

Python (pandas) · Microsoft SQL Server · Power BI

# ▶️ How to Reproduce
Run the Python cleaning steps and load the data into a table named customer.
Open sql/Customer_behavior_analysis.sql in SSMS and run each query.
Open dashboard/Customer_Behavior.pbix in Power BI Desktop.

# 🙏 Acknowledgements

This project was created for learning purposes by following the tutorial and methodology of Amlan Mohanty.

🎥 YouTube: https://www.youtube.com/@amlanmohanty1
💻 GitHub: https://github.com/amlanmohanty1

All credit for the original project idea, dataset walkthrough and approach goes to the creator. This repository is my personal practice implementation.

# 👤 Author

www.linkedin.com/in/vikash-rawat-b86b781a9
