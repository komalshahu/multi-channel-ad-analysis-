# 📊 Marketing Campaign Performance Analysis
This project explores the performance of digital marketing campaigns run across Facebook Ads, Google Ads, and DV360. The analysis is based on a real-world scenario where an e-commerce jewelry brand wants to understand which channels, creatives, and audience strategies drive the most value in terms of CTR, Conversions, and ROI.

🧩 Problem Statement
"An e-commerce brand runs multi-channel ad campaigns. The objective is to evaluate the impact of ad spends and identify key performance drivers (like clicks, conversions, CTR, ROI, etc.) across different platforms."

🎯 Goals
Identify high ROI campaigns by platform, creative, and region

Detect underperforming campaigns based on CTR, CPC, CPM

A/B test ad creatives, channels, and campaign strategies

Measure impact of ad clicks on conversions

Understand weekly/monthly trends

Evaluate long-term relationship between ad spend and conversion

Provide actionable recommendations to optimize marketing budget

📁 Dataset
The dataset contains ad-level metrics such as:

ext_service_name: Advertising platform (Facebook, Google, DV360)

clicks, impressions, media_cost_usd

estimated_conversions

time, channel_name, creative_id, landing_page

🧪 Key Analyses
📈 1. Campaign Metrics
Calculated CTR = clicks / impressions

Calculated CPC = media_cost_usd / clicks

Calculated CPM = (media_cost_usd / impressions) * 1000

✅ 2. Performance Insights
DV360 showed consistently high conversions at a moderate cost

Facebook Ads had slightly better CTR but less efficiency in conversion

Google Ads performance was stable across conversion brackets

📊 3. Conversions by Range
Grouped estimated conversions into buckets:
1–15, 16–30, 31–50, 51–100, 101–250, >250
And visualized count of campaigns in each bracket per platform

🔄 4. Correlation Analysis
Clicks vs Conversions correlation:

DV360 → 1.00

Facebook → 0.999

Google → 0.999

⚖️ 5. A/B Testing
Compared conversion rates across Facebook and Google

T-test p-value: 0.1486 → no significant difference in mean conversions
(We fail to reject the null hypothesis.)

📉 6. Regression (DV360)
Linear regression: estimated_conversions = 0.02 * clicks

Interpretation: Every 100 clicks yield approx. 2 conversions

📆 7. Time-Based Trends
Weekly & Monthly conversions visualized and aggregated

Cost per Conversion calculated by week/month

🔁 8. Long-Term Relationship
Correlation between spend and conversion = 0.616

Cointegration Test p-value = 0.0000
→ Strong long-term stable relationship between ad spend and conversions

🛠️ Tools & Libraries
Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Statsmodels)

Jupyter Notebook

Statistical Tests: Pearson correlation, T-Test, Linear Regression
