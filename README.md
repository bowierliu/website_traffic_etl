# Website Traffic Analysis

## Project Overview
This project implements an ETL (Extract, Transform, Load) pipeline to analyze website traffic data. The analysis uncovers key insights on traffic sources, user behavior, and engagement metrics, providing actionable recommendations to optimize marketing strategies and improve website performance. The project includes data cleaning, transformation, visualization, and detailed insights.

---

## Dataset Description
- **Source**: Kaggle (Simulated Website Traffic Data)
- **Total Records**: 2000
- **Features**:
  - `Page Views`: Number of pages viewed during a session.
  - `Session Duration`: Total duration of the session (minutes).
  - `Bounce Rate`: Percentage of visitors who navigate away after viewing one page.
  - `Traffic Source`: Origin of the traffic (Organic, Paid, Referral, Social, Direct).
  - `Time on Page`: Time spent on a specific page.
  - `Previous Visits`: Number of previous visits by the same user.
  - `Conversion Rate`: Percentage of visitors who completed a desired action (e.g., purchase).
  - `Engagement Score`: A derived metric (Page Views × Session Duration) indicating user engagement.

---

## ETL Process
### 1. **Extract**
- Data was loaded from a Kaggle dataset into a Pandas DataFrame.
- Dataset contains traffic-related metrics for analysis.

### 2. **Transform**
- Cleaned missing and duplicate data.
- Standardized `Traffic Source` values for consistency.
- Derived a new feature, `Engagement Score`, to measure user engagement.

### 3. **Load**
- Transformed data was loaded into a SQLite database for analysis and querying.

---

## Analysis and Insights
### Key Findings:
1. **Traffic Distribution**:
   - Organic traffic contributes the highest number of sessions (786), followed by Paid (428) and Referral (301).
   - Recommendation: Focus on SEO and Paid campaign optimization.

2. **Average Session Duration**:
   - Referral traffic has the highest average session duration (3.13 minutes).
   - Recommendation: Strengthen partnerships with referral sources.

3. **Bounce Rate**:
   - Referral traffic has the lowest bounce rate (26.63%), while Social and Paid traffic have higher rates (~29.6%).
   - Recommendation: Optimize landing pages for Paid and Social campaigns.

4. **High Engagement Pages**:
   - Pages with high engagement scores (>100) are primarily associated with Organic and Paid traffic sources.
   - Recommendation: Analyze successful page designs and replicate best practices.

---

## Visualizations
The following visualizations were created to support the analysis:
- Traffic distribution by source (bar chart).
- Average session duration by source (bar chart).
- Average bounce rate by source (bar chart).
- High engagement pages (scatter plot).
