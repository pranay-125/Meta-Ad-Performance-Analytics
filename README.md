# 📊 Meta Ad Performance Analysis
Facebook & Instagram Marketing Analytics Project

An end-to-end Data Analytics project focused on analyzing the performance of Facebook and Instagram paid advertisements using event-level marketing data.

The project demonstrates how a Data Analyst converts raw marketing data into actionable business insights using Power BI, Excel, SQL, Data Modeling, and DAX.

📌 Project Objective

Marketing teams often run multiple advertising campaigns but struggle to clearly understand:

Which platform performs better
Which audience segments respond the most
Which ad formats generate higher engagement
Where conversion drop-offs occur in the marketing funnel

This project aims to build a data-driven dashboard to help stakeholders make better marketing and budget decisions.

🧠 Business Problem

The marketing team had access to large volumes of raw advertising data, but lacked a centralized system to analyze:

Campaign performance across platforms
Audience engagement patterns
Funnel conversion efficiency
Budget utilization and ROI

Without analytics, decision-making relied mostly on intuition rather than data.

🎯 Business Goals

The analysis focuses on enabling stakeholders to:

✔ Understand campaign performance across Facebook and Instagram
✔ Identify high-performing audiences and ad formats
✔ Detect conversion drop-offs across the funnel
✔ Optimize budget allocation and targeting strategies

🗂 Dataset Overview

The dataset simulates Meta Ads performance data, similar to how Facebook Ads Manager stores campaign interactions.

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

Key fields:

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
