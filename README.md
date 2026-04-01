📊 Meta Ad Performance Analysis
Facebook & Instagram Marketing Analytics Project

An end-to-end Data Analytics project focused on analyzing the performance of Facebook and Instagram paid advertisements using event-level marketing data.

This project demonstrates how a Data Analyst transforms raw marketing data into actionable business insights using Power BI, Excel, SQL, Data Modeling, and DAX.

📌 Project Objective

Marketing teams often run multiple advertising campaigns but struggle to clearly understand:

Which platform performs better
Which audience segments respond the most
Which ad formats generate higher engagement
Where conversion drop-offs occur in the marketing funnel

This project builds a data-driven dashboard to help stakeholders make better marketing and budget decisions.

🧠 Business Problem

The marketing team had access to large volumes of raw advertising data, but lacked a centralized system to analyze:

Campaign performance across platforms
Audience engagement patterns
Funnel conversion efficiency
Budget utilization and ROI

Without analytics, decision-making relied mostly on intuition rather than data.

<img width="845" height="666" alt="Screenshot 2026-04-01 172718" src="https://github.com/user-attachments/assets/c39293db-29f2-4e9b-ba6d-7e8df3a53cfe" />

Data Sources
Table	Description
ad_events	Event-level interactions (impressions, clicks, purchases)
ads	Metadata about ad creatives and targeting
campaigns	Campaign-level strategy and budget details
users	User demographic and interest information
🧩 Data Model

The project uses a Star Schema, which is the standard modeling approach in Business Intelligence systems.

Fact Table

ad_events

Stores all user interactions with advertisements.

Fields include:

event_id
ad_id
user_id
timestamp
event_type
Dimension Tables

ads

ad_platform
ad_type
campaign_id
target_gender
target_age_group

campaigns

campaign_id
campaign_name
start_date
end_date
total_budget

users

user_id
gender
age_group
country
interests
🔗 Table Relationships

The tables are connected using the following relationships:

campaigns.campaign_id → ads.campaign_id

ads.ad_id → ad_events.ad_id

users.user_id → ad_events.user_id

This data model enables multi-dimensional analysis across campaigns, audiences, and ad creatives.

📊 Key KPIs

The dashboard tracks performance using marketing funnel metrics.

KPI	Description
Impressions	Number of times ads were shown
Clicks	Number of user clicks
Engagements	Clicks + Shares + Comments
Purchases	Completed conversions
CTR	Clicks ÷ Impressions
Engagement Rate	Engagements ÷ Impressions
Conversion Rate	Purchases ÷ Clicks
Purchase Rate	Purchases ÷ Impressions
Total Budget	Total campaign spend
Avg Budget per Campaign	Budget allocation efficiency
📊 Dashboard Visualizations

The Power BI dashboard includes multiple analytical views.

Audience Insights
Gender Distribution (Donut Chart)
Age Group Engagement (Bar Chart)
Geographic Insights
Country Performance Map
Time-Based Analysis
Calendar Heat Map (Monthly trends)
Weekly Performance Trend
Hourly Engagement Pattern
Creative Performance
Ad Type Performance Matrix
📈 Key Insights
Funnel Performance
216K Impressions
25.4K Clicks
1.3K Purchases

Strong reach and engagement but conversion efficiency is low.

Audience Insights
Females generate the highest engagement
Age group 18–30 dominates campaign interaction
Ad Format Performance

Best performing formats:

Video Ads
Story Ads

Carousel and Image ads show slightly lower conversion performance.

Geographic Insights

Top engagement regions:

India
United States
Brazil
Germany
United Kingdom
Time-Based Insights

Peak engagement occurs during:

Afternoon and Evening hours

Lowest engagement occurs during:

Early morning (0–5 AM)

💡 Business Recommendations

Based on the analysis:

Allocate more budget to Video and Story ads
Focus campaigns on female users aged 18–30
Schedule ads during afternoon and evening hours
Improve landing pages and retargeting strategies
Prioritize high-engagement markets such as India and the US
🛠 Tools & Technologies
Tool	Purpose
Power BI	Dashboard development and visualization
Excel	Data exploration and preparation
SQL	Data querying and transformation
DAX	KPI calculations
Data Modeling	Star schema design
📁 Repository Structure
Meta-Ad-Performance-Analysis

datasets
 ├── ad_events.csv
 ├── ads.csv
 ├── campaigns.csv
 └── users.csv

documentation
 ├── Business Requirements Document
 ├── Domain Knowledge Document
 └── Dashboard Insights

dashboard
 └── Power BI Dashboard File

presentation
 └── Project Presentation PPT

README.md
🚀 Key Learning Outcomes

This project strengthened my ability to:

Translate business requirements into KPIs
Build scalable data models
Perform funnel-based marketing analytics
Generate actionable business insights
Communicate insights through interactive dashboards

👨‍💻 Author

Pranay Shrivastava

Aspiring Data Analyst | Business Analytics Enthusiast

Skills:

Power BI
SQL
Excel
Data Modeling
Business Analytics

⭐ If you found this project useful

Feel free to star the repository or connect with me on LinkedIn to discuss analytics, dashboards, and data-driven decision making.
