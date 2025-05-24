<h1 align="center">Airline Delay Analytics: AWS Athena + SQL Pipeline for US Flight Performance Insights</h1>

## 📊 Overview

This Excel-based time series forecasting project analyzes 15 years of U.S. hardware and tools retail sales data to generate a 12-month predictive sales forecast. Completed as part of a graduate-level **Supply Chain Analytics** course, the assignment placed me in the role of a **Supply-Chain Analyst** tasked with producing a highly accurate monthly sales forecast to inform internal resource planning—materials, staffing, and financial capacity for the upcoming fiscal year.

The core analysis—including model construction, validation, and communication—was performed in under **90 minutes as part of a timed 3-hour timed project**, simulating a real-world corporate decision-making environment. The task required evaluating industry sales data (Sep 2005–Aug 2020), forecasting future demand (Sep 2020–Aug 2021), and benchmarking against actual 2021 results.

📊 A separate *Forecast vs. Actual Sales* validation sheet is included to compare the forecast against real 2021 Census retail sales figures. This comparison demonstrates forecast realism and business applicability using Mean Absolute Percentage Error (MAPE) and trend visualization.

The final forecast is presented in a concise executive summary tailored for operational stakeholders, delivering clear, actionable insights. Also included is a reusable Time Series Forecasting Playbook authored to document the complete modeling workflow. It serves as both a practical forecasting guide and evidence of applied proficiency in time series forecasting techniques using Excel.

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
  - `Visualizations/` – contains AWS QuickSight charts and Athena-exported CSVs used to generate visual insights:  
    - `Question 1 Visualization.png`, `Visualization 2.png`, ... – QuickSight bar, line, and scatter charts  
    - `CSV 1.csv`, `CSV 4.3.csv`, etc. – Athena query result exports used for chart creation

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

