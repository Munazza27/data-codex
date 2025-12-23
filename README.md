Bear Cart E-Commerce Analytics Project
Insight Summary and Business Recommendations
Hack4Insights 2025 
Team Name: Code Cortex
Date: December 19, 2025 
BearCart is a growing online retail company preparing for its next phase of expansion. While the business collects large volumes of digital and transactional data, its leadership currently lacks clear visibility into customer behavior, marketing effectiveness, and overall revenue performance. To support better decision-making, our team was tasked with cleaning the raw multi-table e-commerce dataset, analyzing key performance areas, and delivering actionable insights through an interactive dashboard.
To address the problem systematically, we divided the overall challenge into logical, sequential parts that directly align with the hackathon objectives and the seven key areas outlined in the problem statement:
Dataset Overview
The following datasets were provided for analysis:
•	website sessions – Contains information about website visits, traffic sources, campaigns, devices, and repeat sessions
•	website pageviews – Records individual page views for each session
•	orders – Stores order-level transaction details
•	order items – Contains product-level details for each order
•	Order item refunds – Includes refund information linked to order items
•	products – Provides product metadata
•	Maven fuzzy actory data dictionary – Reference dataset explaining table structures and fields

How Our Solution Addresses BearCart’s Challenges
We approached the project step by step, starting from raw data and ending with clear business actions. Below is how we solved each part of the problem.
Link to our Notebook:
https://colab.research.google.com/drive/1NR8czWpsODRAHezyqeM19peBhvVr4RrA?usp=sharing

Part 1: Data Preparation & Cleaning
Data cleaning was performed to ensure accuracy, consistency, and reliability of analysis. The following steps were applied across datasets.
1.1 Website Sessions
 Converted date and time fields to datetime format
 Standardized categorical values (e.g., UTM sources, campaigns) by correcting inconsistencies in text case
 Handled missing UTM values by categorizing them as non-campaign traffic
 Verified uniqueness of website_session_id
  Ensured device type and traffic source fields were consistent
 
1.2 Website Pageviews
  Verified multiple pageviews per session as expected behavior
  Converted timestamps to datetime format
  Ensured page URLs were consistently formatted
 Checked for and confirmed absence of missing values
 
1.3 Orders
  Verified uniqueness of order_id
  Rounded monetary values (price and cost) to two decimal places
  Retained missing user_id values without assumptions
  Ensured consistency across financial fields
 
1.4 Order Items
  Validated price and cost fields
  Ensured correct identification of primary items
  Confirmed absence of missing or duplicate records
 
1.5 Order Item Refunds
  Confirmed refund records were transaction-level
  Allowed duplicate order IDs as valid (multiple refunds per order possible)
  Standardized date and monetary formats
 
1.6 Products
  Converted product creation dates to datetime format
  Verified uniqueness of product identifiers
 
The cleaned datasets formed the foundation for further analysis.
Part 2: Website & Traffic Analysis 
 2.1 Website Traffic Analysis
 Analysis of website sessions revealed trends in traffic volume, traffic sources, and device usage. Desktop traffic demonstrated higher engagement compared to mobile traffic, indicating potential usability differences across devices.
  2.2 Conversion Behavior
 Session-to-order conversion analysis showed variations across traffic sources and repeat sessions. Repeat sessions exhibited higher conversion likelihood compared to first-time visits.
 2.3 Revenue & Product Performance
 Revenue analysis highlighted dependence on a limited number of top-performing products. Average Order Value (AOV) remained relatively stable, indicating consistent pricing behavior.
 2.4 Refund Analysis
 Refund data indicated that while refunds occur infrequently, they can significantly affect net revenue for specific products and periods


Part 3: Conversion Analysis (The core of business impact)
What we analyzed: 
•	Sessions compared to actual orders 
•	Overall conversion rate 
•	Conversion performance for each channel
Business question answered:
“Are visitors actually turning into paying customers?” 
Outcome: 
•	Highlights which traffic sources bring high-quality visitors 
•	Shows where potential customers are dropping off 
•	Helps decide where to spend marketing budget wisely



Key Performance Indicators (KPIs)
Total Sessions
 Measures the total number of website visits during the analysis period. It helps assess overall traffic volume and the effectiveness of customer acquisition efforts.
Total Orders
 Represents the number of completed purchases. This metric reflects the platform’s sales performance.
Conversion Rate
 Calculated as the ratio of total orders to total website sessions. It indicates how effectively website visits are converted into purchases.
Average Order Value (AOV)
 Measures the average revenue generated per order. It provides insights into customer spending patterns and pricing strategy.
Refund Rate
 Represents the proportion of orders that were refunded. A higher refund rate may indicate product, pricing, or customer experience issues.
Total Revenue
 Captures the total sales value generated from all orders. It is a key indicator of overall business growth.
Part 4: Revenue & Order Value Analysis
What we analyzed: 
•	Total revenue 
•	Revenue trends over time 
•	Average order value (AOV)
Business question answered:
“How is the business doing financially?” 
Outcome: 
•	Clear view of revenue growth or any stagnation 
•	Spots issues with low average order values 
•	Provides evidence for pricing or bundling decisions
Example insight:
“Order numbers are steady, but AOV is quite low—there’s room to encourage upselling or bundling.” 
Dashboard view: 
•	KPI cards for total revenue and AOV 
•	A line chart showing revenue trend
Value to BearCart:
Leadership gets a real sense of how money is coming in, beyond just counting orders.
Part 5: Product Performance & Refund Analysis
What we analyzed: 
•	Revenue generated by each product 
•	Top-performing vs underperforming products 
•	Refund rates and total refund amounts
Business question answered:
“Which products are driving profit, and which ones are causing losses?” 
Outcome: 
•	Quickly identifies the best-selling and most profitable items 
•	Flags products with unusually high refund rates 
•	Helps improve product quality and customer satisfaction
Example insight:
“Some of our highest-revenue products also have the highest refunds—this could point to quality issues or mismatched expectations.” 
Dashboard view: 
•	Bar chart for top products by revenue 
•	KPI card for overall refund rate 
•	Table showing product-level refund details
Value to BearCart:
The team can address problematic products early and protect the brand’s reputation.
Part 6: Insight Generation & Business Recommendations
What we Did: 
•	Not just numbers and charts, but clear actionable recommendations 
•	Explained what the data shows, why it matters, and what to do next
Outcome: 
•	Management receives insights they can act on immediately 
•	Data directly translates into real business improvements 
•	Decisions are based on evidence rather than guesswork
Example:
“Shift more budget toward organic search since it converts well, and rework paid social campaigns to improve targeting.”
Final Dashboard Overview 
The dashboard pulls everything together in one interactive view with these main sections: 
1.	Overview – Key metrics like sessions, orders, conversion rate, and revenue 
2.	Traffic – Session trends and channel breakdown 
3.	Conversion – Funnel and channel-wise performance 
4.	Revenue – Revenue and AOV trends 
5.	Products & Refunds – Top products and refund impact
Purpose:
It’s designed to be easy for decision-makers to use, not overly technical
Project Summary
Our solution takes messy e-commerce data and turns it into a clear, reliable decision-making tool that helps BearCart bring in better traffic, boost conversions, grow revenue, and lower refunds.
