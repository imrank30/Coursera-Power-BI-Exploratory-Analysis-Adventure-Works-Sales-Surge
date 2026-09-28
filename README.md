This project analyzes an unexpected surge in sales data for Adventure Works using Microsoft Power BI Desktop. The objective was to identify peak sales dates, discover underlying root causes for sales anomalies using automated analytics tools, and deliver data-driven visual reports to assist management decision-making.

🛠️ Tools & Techniques Used
Tool: Microsoft Power BI Desktop

Data Visualizations: Time Series Line Chart, Scatter Plot, Donut Charts, Tree Chart 

📊 Visual Analysis & Findings
1. Identifying the Sales Anomalies
•	Visual Description: A time-series line chart mapping Order Date on the X-axis against Sum of Order Total on the Y-axis.
•	What I Found:
o	Successfully isolated two distinct high-volume sales spike days in the dataset.
o	Pinpointed March 7th as the single highest sales surge date, triggering the root-cause investigation.
________________________________________
2. Segmenting Products with K-Means Clustering
•	Visual Description: A scatter plot configured with Sum of Order Total (X-axis) and Sum of Product Price (Y-axis) across high-cardinality Product Name records. Power BI's automated clustering was applied to group products into 3 distinct operational segments.
•	What I Found:
o	Cluster 1: Entry-level / low-priced items (32K total revenue).
o	Cluster 2: Mid-tier performance items (39.4K total revenue).
o	Cluster 3: High-value flagship items (77K total revenue).
o	Structuring products into 3 distinct clusters provided machine-learning context to assist Power BI's Analyze engine in isolating key drivers.
________________________________________
3. Measuring Revenue Distribution Across Clusters
•	Visual Description: A treemap visual displaying total revenue volume contributed by each generated product cluster (Cluster 1, Cluster 2, Cluster 3).
•	What I Found:
o	Quantified revenue performance across groups, revealing that Cluster 3 generated the dominant portion of total volume (77K), followed by Cluster 2 (39.4K) and Cluster 1 (32K).
________________________________________
4. Analyzing Low-Cardinality Attributes (Product Sizing)
•	Visual Description: A donut chart analyzing revenue distribution across the Product Size attribute (a low-cardinality field with 2 distinct values: M and L).
•	What I Found:
o	Revealed that Medium (M) size products heavily dominated sales volume (96K or 65.22%) compared to Large (L) size ( 51K or 34.78%).
________________________________________
5. Automated Root Cause Analysis (Explain the Increase)
•	Visual Description: An automated waterfall variance chart generated using Power BI's Explain the Increase tool on the peak sales date (comparing March 7th against March 6th).
•	What I Found:
o	Isolated the specific product categories driving day-over-day variance.
o	Proved that the surge was overwhelmingly driven by high volume in Road Bikes, with secondary lifts coming from E-Bikes and Mountain Bikes.
o	Confirmed 3 shared contributory factors across both peak sales surge dates.
________________________________________
💡 Core Business Recommendations
1.	Targeted Inventory Allocation: Supply chain and logistics teams should prioritize inventory availability for Medium-framed Road Bikes ahead of future marketing promotions.
2.	Promotional Focus: Focus marketing campaigns on Cluster 3 (high-value flagship items), as they generate the largest revenue contribution during peak demand surges.

