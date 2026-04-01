<h1>📊 Meta Ad Performance Analysis</h1>

<h3>Facebook & Instagram Marketing Analytics Project</h3>

<p>
An <strong>end-to-end Data Analytics project</strong> focused on analyzing the performance of 
<strong>Facebook and Instagram paid advertisements</strong> using event-level marketing data.
</p>

<p>
This project demonstrates how a <strong>Data Analyst transforms raw marketing data into actionable business insights</strong> 
using <strong>Power BI, Excel, SQL, Data Modeling, and DAX</strong>.
</p>

<hr>

<h2>📌 Project Objective</h2>

<p>
Marketing teams often run multiple advertising campaigns but struggle to clearly understand:
</p>

<ul>
<li>Which <strong>platform performs better</strong></li>
<li>Which <strong>audience segments respond the most</strong></li>
<li>Which <strong>ad formats generate higher engagement</strong></li>
<li>Where <strong>conversion drop-offs occur in the marketing funnel</strong></li>
</ul>

<p>
This project builds a <strong>data-driven dashboard</strong> to help stakeholders make 
<strong>better marketing and budget decisions</strong>.
</p>

<hr>

<h2>🧠 Business Problem</h2>

<p>
The marketing team had access to <strong>large volumes of raw advertising data</strong>, 
but lacked a centralized system to analyze:
</p>

<ul>
<li>Campaign performance across platforms</li>
<li>Audience engagement patterns</li>
<li>Funnel conversion efficiency</li>
<li>Budget utilization and ROI</li>
</ul>

<p>
Without analytics, decision-making relied mostly on <strong>intuition rather than data</strong>.
</p>

<hr>

<h2>🎯 Business Goals</h2>

<ul>
<li>Understand campaign performance across <strong>Facebook and Instagram</strong></li>
<li>Identify <strong>high-performing audiences and ad formats</strong></li>
<li>Detect <strong>conversion drop-offs across the funnel</strong></li>
<li>Optimize <strong>budget allocation and targeting strategies</strong></li>
</ul>

<hr>

<h2>🗂 Dataset Overview</h2>

<p>
The dataset simulates <strong>Meta Ads performance data</strong>, similar to how Facebook Ads Manager stores campaign interactions.
</p>

<h3>Data Sources</h3>

<table border="1" cellpadding="8" cellspacing="0">
<tr>
<th>Table</th>
<th>Description</th>
</tr>

<tr>
<td>ad_events</td>
<td>Event-level interactions (impressions, clicks, purchases)</td>
</tr>

<tr>
<td>ads</td>
<td>Metadata about ad creatives and targeting</td>
</tr>

<tr>
<td>campaigns</td>
<td>Campaign-level strategy and budget details</td>
</tr>

<tr>
<td>users</td>
<td>User demographic and interest information</td>
</tr>
</table>

<hr>

<h2>🧩 Data Model</h2>

<p>
The project uses a <strong>Star Schema</strong>, which is the standard modeling approach in Business Intelligence systems.
</p>

<h3>Fact Table</h3>

<p><strong>ad_events</strong></p>

<p>Stores all user interactions with advertisements.</p>

<ul>
<li>event_id</li>
<li>ad_id</li>
<li>user_id</li>
<li>timestamp</li>
<li>event_type</li>
</ul>

<h3>Dimension Tables</h3>

<p><strong>ads</strong></p>

<ul>
<li>ad_platform</li>
<li>ad_type</li>
<li>campaign_id</li>
<li>target_gender</li>
<li>target_age_group</li>
</ul>

<p><strong>campaigns</strong></p>

<ul>
<li>campaign_id</li>
<li>campaign_name</li>
<li>start_date</li>
<li>end_date</li>
<li>total_budget</li>
</ul>

<p><strong>users</strong></p>

<ul>
<li>user_id</li>
<li>gender</li>
<li>age_group</li>
<li>country</li>
<li>interests</li>
</ul>

<hr>

<h2>🔗 Table Relationships</h2>

<p>The tables are connected using the following relationships:</p>

<pre>
campaigns.campaign_id → ads.campaign_id
ads.ad_id → ad_events.ad_id
users.user_id → ad_events.user_id
</pre>

<p>
This data model enables <strong>multi-dimensional analysis across campaigns, audiences, and ad creatives</strong>.
</p>

<hr>

<h2>📊 Key KPIs</h2>

<table border="1" cellpadding="8" cellspacing="0">
<tr>
<th>KPI</th>
<th>Description</th>
</tr>

<tr>
<td>Impressions</td>
<td>Number of times ads were shown</td>
</tr>

<tr>
<td>Clicks</td>
<td>Number of user clicks</td>
</tr>

<tr>
<td>Engagements</td>
<td>Clicks + Shares + Comments</td>
</tr>

<tr>
<td>Purchases</td>
<td>Completed conversions</td>
</tr>

<tr>
<td>CTR</td>
<td>Clicks ÷ Impressions</td>
</tr>

<tr>
<td>Engagement Rate</td>
<td>Engagements ÷ Impressions</td>
</tr>

<tr>
<td>Conversion Rate</td>
<td>Purchases ÷ Clicks</td>
</tr>

<tr>
<td>Purchase Rate</td>
<td>Purchases ÷ Impressions</td>
</tr>

<tr>
<td>Total Budget</td>
<td>Total campaign spend</td>
</tr>

<tr>
<td>Avg Budget per Campaign</td>
<td>Budget allocation efficiency</td>
</tr>
</table>

<hr>

<h2>📊 Dashboard Visualizations</h2>

<h3>Audience Insights</h3>

<ul>
<li>Gender Distribution (Donut Chart)</li>
<li>Age Group Engagement (Bar Chart)</li>
</ul>

<h3>Geographic Insights</h3>

<ul>
<li>Country Performance Map</li>
</ul>

<h3>Time-Based Analysis</h3>

<ul>
<li>Calendar Heat Map (Monthly trends)</li>
<li>Weekly Performance Trend</li>
<li>Hourly Engagement Pattern</li>
</ul>

<h3>Creative Performance</h3>

<ul>
<li>Ad Type Performance Matrix</li>
</ul>

<hr>

<h2>📈 Key Insights</h2>

<h3>Funnel Performance</h3>

<ul>
<li>216K Impressions</li>
<li>25.4K Clicks</li>
<li>1.3K Purchases</li>
</ul>

<p>
Strong reach and engagement but <strong>conversion efficiency is low</strong>.
</p>

<h3>Audience Insights</h3>

<ul>
<li>Females generate the <strong>highest engagement</strong></li>
<li>Age group <strong>18–30 dominates campaign interaction</strong></li>
</ul>

<h3>Ad Format Performance</h3>

<ul>
<li>Video Ads perform the best</li>
<li>Story Ads also show strong performance</li>
<li>Carousel and Image ads show slightly lower conversions</li>
</ul>

<h3>Geographic Insights</h3>

<ul>
<li>India</li>
<li>United States</li>
<li>Brazil</li>
<li>Germany</li>
<li>United Kingdom</li>
</ul>

<h3>Time-Based Insights</h3>

<p>
Peak engagement occurs during <strong>afternoon and evening hours</strong>.
</p>

<p>
Lowest engagement occurs during <strong>early morning hours (0–5 AM)</strong>.
</p>

<hr>

<h2>💡 Business Recommendations</h2>

<ul>
<li>Allocate more budget to <strong>Video and Story ads</strong></li>
<li>Focus campaigns on <strong>female users aged 18–30</strong></li>
<li>Schedule ads during <strong>afternoon and evening hours</strong></li>
<li>Improve <strong>landing pages and retargeting strategies</strong></li>
<li>Prioritize high-engagement markets such as <strong>India and the US</strong></li>
</ul>

<hr>

<h2>👨‍💻 Author</h2>

<p><strong>Pranay Shrivastava</strong></p>

<p>
Aspiring <strong>Data Analyst | Business Analytics Enthusiast</strong>
</p>

<h3>Skills</h3>

<ul>
<li>Power BI</li>
<li>SQL</li>
<li>Excel</li>
<li>Data Modeling</li>
<li>Business Analytics</li>
</ul>
