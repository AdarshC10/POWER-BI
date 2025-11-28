
# 📊 Meta Ad Performance Dashboard — Power BI

This project presents an end-to-end analytical dashboard to evaluate performance trends of **Meta (Facebook & Instagram) advertising campaigns**.  
The dashboard enables marketing teams to make **data-driven decisions** by highlighting insights on **engagement, conversions, audience behavior, and budget utilization**.

---

## 🚀 Project Overview

Companies invest heavily in digital ads, but identifying **what drives the most conversions and engagement** remains a challenge.  
To address this, I built an **interactive Power BI dashboard** that visualizes ad performance across **platforms, demographics, interests, and time periods** to uncover meaningful patterns.

---

## 🎯 Key Features

- 📌 KPI tracking — Impressions, Clicks, Shares, Comments, Purchases, Engagements  
- 📌 Budget analytics — Total Spend & Avg. Budget per Campaign  
- 📌 Performance breakdown by **platform, age group, country, gender, and interests**  
- 📌 Trend analysis — **Daily, monthly, and hourly fluctuations in engagement**  
- 📌 Campaign drill-down with interactive slicers  
- 📌 Identification of **best-performing ads and audience segments**

---

## 🧠 Business Insights Gained

🔹 Video ads deliver the highest conversion success  
🔹 Purchases and CTR vary sharply by **age group and interests**  
🔹 Engagement rate peaks during **specific hours of the day**  
🔹 USA, UK & Canada produce the strongest purchase rate  
🔹 Optimal budget allocation improves campaign performance significantly  

> These insights help optimize **targeting, timing, ad formats, and budget distribution**.

---

## 📷 Dashboard Preview
<img width="986" height="564" alt="image" src="https://github.com/user-attachments/assets/b653df82-b6f0-4b45-ba5f-70ac3ebc8692" />
<img width="987" height="565" alt="image" src="https://github.com/user-attachments/assets/fdd8de75-526a-4327-93b5-1290d2431df6" />
<img width="987" height="565" alt="image" src="https://github.com/user-attachments/assets/3b103fbd-da76-4e08-bb6b-8081a70213ac" />


---

## 🛠 Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI** | Dashboard Creation |
| **Power Query** | Data Cleaning & Transformation |
| **DAX** | KPIs Calculations |
| **Excel / CSV** | Dataset Source |

---

## 📑 DAX Measures Used (Samples)

```DAX
CTR = DIVIDE([Clicks], [Impressions])
Engagement Rate = DIVIDE([Engagements], [Impressions])
Conversion Rate = DIVIDE([Purchases], [Clicks])
Avg Budget per Campaign = AVERAGE('Campaigns'[Total Budget])
```
---

## 🙌 About Me

Aspiring Data Analyst | Data Scientist | Power BI | SQL | Python | Excel

📩 Email: adarshcrv@gmail.com
🔗 LinkedIn: https://www.linkedin.com/in/adarsh-c-developer




