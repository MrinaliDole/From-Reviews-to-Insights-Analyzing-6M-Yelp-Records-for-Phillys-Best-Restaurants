# From-Reviews-to-Insights-Analyzing-6M-Yelp-Records-for-Philly-s-Best-Restaurants

📌 Project Overview

As part of our Enterprise Data Management  course, our team built a 360° data pipeline to analyze the Yelp public dataset (6M+ records). The objective was to identify top-performing restaurants in Philadelphia by combining data engineering (Azure SQL) with exploratory analytics (Python).

We designed a relational schema in Azure SQL Server, loaded and filtered the dataset via SQL queries, and then used Python (Pandas, Matplotlib, Seaborn) for in-depth analysis. The project demonstrated how structured pipelines can turn messy, real-world data into business-relevant insights.

📝 Concise Narrative Summary

Our team extracted and cleaned millions of Yelp reviews and business records, structured them into Azure SQL tables, and queried them to focus on Philadelphia restaurants. We applied filters (≥4.0 stars and 100+ reviews) for quality assurance, then pulled results into Python for deeper analysis. Using Pandas and visualization libraries, we uncovered customer sentiment trends, cuisine popularity, and restaurant rankings.

This workflow simulated a real-world data engineering → analytics pipeline, showing how SQL and Python can complement each other to deliver insights for both consumers (finding high-quality dining options) and restaurant owners (benchmarking performance).

📦 Key Deliverables

Data Loading Notebook (mini-project-group-4-load.ipynb) – Python scripts to parse raw Yelp data and load into Azure SQL.

SQL Query Notebook (Mini_Project_Group_4_query.ipynb) – SQL queries for filtering businesses, reviews, and users.

Azure SQL Database – relational schema with business, review, user, tip, check-in tables.

Python EDA Outputs – cuisine trends, restaurant rankings, and customer review insights.

📊 Insights & Outcomes
Top Cuisines in Philadelphia
| Cuisine Category | Restaurant Count |
| ---------------- | ---------------- |
| Pizza            | 935              |
| Mexican          | 728              |
| Chinese          | 708              |
| Italian          | 328              |
| American (New)   | 247              |


Top Restaurants in Philadelphia
| Restaurant Name               | Stars | Reviews |
| ----------------------------- | ----- | ------- |
| St Yared Ethiopian Restaurant | 5.0   | 250     |
| Sundae’s Ice Cream & Coffee   | 5.0   | 225     |
| Ali’i Poke Indy               | 5.0   | 223     |
| Tlaolli                       | 5.0   | 209     |
| Subito                        | 5.0   | 203     |


📝 Engagement & Review Patterns

Philadelphia had ~666K reviews, one of the most active cities in the dataset.

Restaurants with <50 reviews often had inflated 5.0 ratings; those with >200 reviews stabilized at 4.2–4.4 stars.

Elite Yelp users contributed ~15% of reviews, averaging 2× more “useful” votes.

Negative reviews were ~30% longer than positive ones.

Seasonal spikes appeared in Nov–Dec, especially for family dining and fine dining cuisines.

🛠️ Tools & Methods

Data Source: Yelp Kaggle dataset (~6M+ records)

Data Engineering: Python (Pandas, JSON parsing) → Azure SQL Server (pyodbc)

Database Design: Relational schema (business, review, user, tip, check-in)

SQL Analytics: filtering, joins, aggregations for location and category subsets

Python Analytics: Pandas, Matplotlib, Seaborn for EDA & visualization

Business Logic: Weighted ranking (rating × review count) for top restaurants

🌍 Business Impact

Consumers: Identified consistently high-quality restaurants for dining decisions.

Restaurant Owners: Benchmarked performance against top competitors in Philadelphia.

Yelp/Product Teams: Demonstrated how structured pipelines can improve recommendation systems and search features.

🔬 Technical Depth 

Built a Python → SQL pipeline to parse raw JSON into normalized tables.

Designed a relational schema in Azure SQL mirroring Yelp’s dataset.

Applied complex SQL queries to filter city, category, and rating thresholds.

Conducted EDA in Python, analyzing distributions, correlations, and trends.

Balanced data engineering scalability with analytics storytelling.

📈 Dashboard / Visualization Highlights

Cuisine Popularity Charts – Pizza, Mexican, and Chinese led in volume.

Top Restaurant Rankings – weighted ratings balanced stars vs. volume.

Review Trends – spikes around holidays; negative reviews longer on average.

User Engagement Analysis – elite users shaped review quality and visibility.
