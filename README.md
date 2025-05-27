<h1 align="center">Airline Delay Analytics: AWS Athena + SQL Pipeline for US Flight Performance Insights</h1>

## 📊 Overview
This project analyzes U.S. airline on-time performance using data from the U.S. Department of Transportation (Bureau of Transportation Statistics). The dataset—over **500,000 flight records** spanning five years—was queried using AWS Athena after being processed through AWS Glue Crawlers and hosted on S3. Visualizations were created with Amazon QuickSight.

The project was part of a capstone assignment in a Business Analytics program's *Business Analysis with Structured Data* course. It was completed in approximately **24 hours**, under intense time constraints, while balancing multiple concurrent deliverables. Despite receiving a messy and incomplete dataset, I engineered a full-stack cloud-native analytics pipeline and produced a professional report with executive-level insights using only SQL and AWS-native tools.

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
- Designed and deployed a complete data analysis workflow using AWS cloud tools on 500K+ flight records.
- Delivered insight-driven SQL analytics using AWS Athena and clean query logic to solve business problems under real-world data limitations.
- Applied creative thinking to compensate for missing fields, including estimating aircraft age via `tail_number` frequency and restructuring analysis prompts to suit available data.
- Identified flaws in the dataset (e.g., 100% weather delay rates, missing time-of-day info) and clearly communicated caveats to stakeholders.
- Delivered a visually supported, executive-ready final report with actionable business recommendations under tight deadline pressure.

## 📁 Project Structure

- `Datasets/`  
  - `Flights On Time Performance Beginning January 2018–2023.zip` – compressed archive containing the raw dataset and official data dictionary:  
    - `OTP_2018_1_to_2023_1.csv` – raw on-time flight performance data from U.S. DOT  
    - `OTP_dataset_readme.html` – official data dictionary from the Bureau of Transportation Statistics  

- `Outputs/`  
  - `A1 - Analysis of Carrier On-Time Performance by Awale Abdi.pdf` – full executive-style report with visual insights and findings  
  - `A1 - Analysis of Carrier On-Time Performance by Awale Abdi-1.txt` – well-documented SQL queries used in Athena  
  - `README.md` – project overview, methodology, and actionable insights summary  
  - `Visualizations/` – collection of supporting visual assets  
    - Amazon QuickSight charts (bar charts, line graphs, scatterplots)  
    - Athena-exported CSVs used to build visualizations (not all used)  

## 🧩 Challenges Faced
- Dataset limited to one month (January 2023) — no seasonal patterns or year-over-year trends possible.
- Missing fields: airline names, time-of-day, passenger counts, delay reasons by cause.
- Data contained anomalies (e.g., 100% weather delay at certain airports), requiring interpretive caution and framing.

## 📈 Actionable Insights
- "AA" (American Airlines) led in flight volume with 138.9K recorded flight segments in Jan 2023 (includes recurring and code-share flights).
- Day 5 (Friday) showed the lowest average delay times among all weekdays.
- No strong evidence found linking higher aircraft usage (proxy for age) to increased delays.
- Recommended significant data quality improvements for better analysis of passenger trends and delay attribution.

## 🔗 Data Source
- [US DOT Bureau of Transportation Statistics](https://www.transtats.bts.gov/Fields.asp?gnoyr_VQ=FGJ)

---

### **Contact Me**

For questions, collaborations, or opportunities:

- 📧 Awaleiabdi@outlook.com  
- 💼 [LinkedIn – Awale Abdi](https://www.linkedin.com/in/awale-abdi/)
