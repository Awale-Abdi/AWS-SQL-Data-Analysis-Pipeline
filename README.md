# Airline Delay Analytics: AWS Athena + SQL Pipeline for US Flight Performance Insights

## 📊 Overview
This project analyzes U.S. airline on-time performance using data from the U.S. Department of Transportation (Bureau of Transportation Statistics). The dataset was queried using AWS Athena after being processed through AWS Glue Crawlers and hosted on S3. Visualizations were created with Amazon QuickSight.

The project was part of a capstone assignment in a Business Analytics program. I was required to answer five key business questions related to airline carrier performance using only SQL and cloud-native tools. Despite data limitations (e.g., missing date ranges, lack of time-of-day fields, no passenger data), I built creative workarounds to derive actionable insights for executive stakeholders.

## 📌 Key Business Questions Answered
1. **Top Airlines by Year** – Which carriers flew the most, and what patterns emerged?
2. **Best Time to Minimize Delays** – Which day of the week sees the fewest delays?
3. **Plane Age & Delay Risk** – Do older planes correlate with higher delay times?
4. **Flight Volume Over Time** – How does flight traffic between locations change?
5. **Weather-Related Delays** – What percentage of delays were weather-induced at each airport?

## 🧠 Methodology
- **Cloud Stack**: AWS S3, Glue Crawler, Athena, QuickSight
- **Query Language**: ANSI SQL
- **Dataset**: U.S. DOT On-Time Performance (Jan 2023 snapshot)
- **Tools Used**: AWS Learner Lab, Athena Query Editor, QuickSight

## ⚙️ Project Highlights
- Created a schema via AWS Glue to parse raw CSV flight data.
- Ran multiple complex SQL queries to transform raw records into business insights.
- Incorporated creative logic to infer insights where direct fields were absent (e.g., estimating aircraft age from `tail_number` frequency).
- Maintained SQL best practices: formatted code, added inline comments, grouped logic cleanly.
- Produced an executive-style report summarizing trends, anomalies, and actionable recommendations.

## 🧩 Challenges Faced
- Dataset limited to January 2023 (no seasonal trends possible).
- Missing fields: passenger counts, flight time-of-day, full airline names.
- Skewed results (e.g., 100% of flights delayed by weather) prompted cautionary interpretation.

## 📈 Actionable Insights
- "AA" (American Airlines) led in flight count with 138.9K flights in January 2023.
- Day 5 (Friday) had the fewest average delays during the month.
- No strong correlation found between inferred aircraft age and delays.
- Urgent need for more complete and structured data collection by agencies.

## 📁 Project Structure
