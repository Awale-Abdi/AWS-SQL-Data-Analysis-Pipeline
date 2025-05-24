<h1 align="center">Airline Delay Analytics: AWS Athena + SQL Pipeline for US Flight Performance Insights</h1>

## 📊 Overview
This project analyzes U.S. airline on-time performance using data from the U.S. Department of Transportation (Bureau of Transportation Statistics). The dataset was queried using AWS Athena after being processed through AWS Glue Crawlers and hosted on S3. Visualizations were created with Amazon QuickSight.

The project was part of a capstone assignment in a Business Analytics program, completed under significant time constraints—less than two days—while managing other concurrent coursework and deliverables. Despite this, I delivered a full-stack analytical solution using only SQL and cloud-native tools to extract actionable insights for executive stakeholders.

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


## 📁 Project Structure

- `Datasets/`  
  - `Flights On Time Performance Beginning January 2018–2023.zip` – compressed archive containing the raw dataset and official data dictionary:  
    - `OTP_2018_1_to_2023_1.csv` – raw on-time flight performance data from U.S. DOT  
    - `OTP_dataset_readme.html` – official data dictionary from the Bureau of Transportation Statistics  

- `Outputs/`  
  - `A1 - Analysis of Carrier On-Time Performance by Awale Abdi.pdf` – full executive-style report with visual insights and findings  
  - `A1 - Analysis of Carrier On-Time Performance by Awale Abdi-1.txt` – well-documented SQL queries used in Athena  
  - `README.md` – project overview, methodology, and actionable insights summary  

- `Visualizations/` – organized into two subfolders:
  - `Quicksight Visualizations/` – exported charts from Amazon QuickSight  
    - Includes bar charts, line graphs, scatterplots, and other visuals used in the final report  
  - `Various CSVs Generated for Making Visualizations (not all used)/` – Athena query result exports  
    - Contains raw data slices prepared for charting and intermediate analysis  


## 🧩 Challenges Faced
- Dataset limited to January 2023 (no seasonal trends possible).
- Missing fields: passenger counts, flight time-of-day, full airline names.
- Skewed results (e.g., 100% of flights delayed by weather) prompted cautionary interpretation.

## 📈 Actionable Insights
- "AA" (American Airlines) led in flight count with 138.9K flights in January 2023.
- Day 5 (Friday) had the fewest average delays during the month.
- No strong correlation found between inferred aircraft age and delays.
- Urgent need for more complete and structured data collection by agencies.

## 🔗 Data Source
- [US DOT Bureau of Transportation Statistics](https://www.transtats.bts.gov/Fields.asp?gnoyr_VQ=FGJ)

---

### **Contact Me**

For questions or collaboration, reach out via:

- Awaleiabdi@outlook.com  
- [LinkedIn](https://www.linkedin.com/in/awale-abdi/)

