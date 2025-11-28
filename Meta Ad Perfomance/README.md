# 📱 Meta Ad Performance Dashboard

[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Meta](https://img.shields.io/badge/Meta-0081FB?logo=meta&logoColor=white)](https://www.meta.com/)
[![DAX](https://img.shields.io/badge/DAX-Analytics-blue)](https://dax.guide/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

An interactive Power BI dashboard for analyzing advertising campaign performance across Meta platforms (Facebook & Instagram). Track impressions, engagement, conversions, and ROI to make data-driven marketing decisions.

<img width="972" height="551" alt="image" src="https://github.com/user-attachments/assets/d35f625d-819a-4af0-9a69-a6b1f0bc2d03" />
<img width="968" height="552" alt="image" src="https://github.com/user-attachments/assets/4858d723-7632-4d3f-9cca-f086cc05c1e8" />
<img width="970" height="553" alt="image" src="https://github.com/user-attachments/assets/48f7da2d-f19e-424f-a0ab-1536b2b5ff33" />


---

## 📌 Project Overview

The **Meta Ad Performance Dashboard** is a comprehensive analytical solution that evaluates advertising campaigns across Facebook and Instagram. It provides real-time insights into how different ad types, demographics, regions, and campaigns contribute to key marketing metrics including:

- 👁️ Impressions & Reach
- 🖱️ Clicks & CTR
- 💬 Engagement & Interactions
- 🛒 Conversions & Purchases
- 💰 Budget & ROI

This dashboard empowers marketing teams to optimize targeting strategies, improve budget allocation, and maximize campaign effectiveness.

---

## 🎯 Key Objectives

- ✅ **Monitor** ad campaign performance in real time across Meta platforms
- ✅ **Identify** the most responsive demographics (age, gender, location)
- ✅ **Evaluate** which ad types (video, image, stories, carousel) produce the highest ROI
- ✅ **Track** engagement and conversion patterns across time periods
- ✅ **Optimize** budget allocation and targeting strategy based on data insights

---

## 🔍 Key Insights

Based on dashboard analysis:

| Insight | Finding |
|---------|---------|
| 📊 **Engagement vs Conversion** | High engagement rate vs lower conversion rate indicates strong attention but need for improved conversion strategy |
| 👥 **Top Demographics** | Age group 25–35 produces highest engagement; ideal target range |
| 🚺 **Gender Performance** | Female audience shows slightly higher interaction compared to male |
| 🎬 **Ad Format Performance** | Video ads lead in engagement; carousel ads show strong conversion |
| 🌍 **Top Regions** | North America and Europe are highest-performing regions |
| ⏰ **Optimal Timing** | Evening hours produce highest engagement |

---

## 🛠️ Tools & Technologies

| Technology | Purpose |
|------------|---------|
| **Power BI Desktop** | Dashboard creation & data visualization |
| **DAX** | Calculated columns, measures & KPIs |
| **Power Query** | Data transformation & cleaning |
| **Excel / CSV** | Data storage & preprocessing |
| **Meta Campaign Data** | Source dataset from Facebook Ads Manager |

---

## 📊 Dashboard Features

### 📈 Key Performance Indicators (KPIs)
- **Reach Metrics:** Impressions, Reach
- **Engagement Metrics:** Clicks, Shares, Comments, Total Engagements
- **Conversion Metrics:** Conversions, Purchases
- **Performance Ratios:** CTR, Engagement Rate, Conversion Rate, Purchase Rate
- **Budget Metrics:** Total Budget, Average Budget per Campaign

### 🎯 Interactive Visualizations

- 👥 **Demographic Analysis:** Performance breakdown by gender & target age groups
- 🌍 **Geographic Distribution:** Engagement mapping by country
- 📅 **Temporal Analysis:** Monthly, weekly, and hourly campaign performance
- 🖼️ **Ad Type Comparison:** Metrics across image, video, story & carousel formats
- 🔄 **Dynamic Filters:**
  - Measure Selection (Engagement, Clicks, CTR, etc.)
  - Campaign Name
  - Target Interests

---

## 🗂️ Data Model Structure

The dashboard uses a **Star Schema** for optimal query performance:

```
Fact_CampaignMetrics (Center)
├── Dim_Campaign      → Campaign ID, Name, Target Interests
├── Dim_Demographics  → Age Groups, Gender
├── Dim_Country       → Geographic information
└── Dim_Time          → Month, Week, Day, Hour
```

**Fact Table:** `Fact_CampaignMetrics`
- Impressions, Clicks, Shares, Comments, Engagements
- Conversions, Purchases
- Budget, Spend

**Dimension Tables:**
- `Dim_Campaign` - Campaign details and targeting
- `Dim_Demographics` - Age and gender segments
- `Dim_Country` - Geographic regions
- `Dim_Time` - Time-based analysis dimensions

---

## 💼 Business Impact

| Impact Area | Benefit |
|-------------|---------|
| 📊 **Marketing Optimization** | Identify high-performing ad formats & demographics |
| 💰 **Budget Efficiency** | Data-driven budgeting to maximize ROI |
| 🎯 **Targeting Strategy** | Refined customer segmentation & personalization |
| 📈 **Performance Tracking** | Improved visibility for management and marketing teams |
| 🧠 **Decision-making** | Actionable insights from historical and real-time data |

### ROI Improvements
- **Better targeting** = Lower cost per acquisition
- **Optimized ad formats** = Higher engagement rates
- **Strategic timing** = Maximum campaign impact
- **Demographic insights** = Precise audience reach


---

## 📁 Project Structure

```
meta-ad-performance-dashboard/
│
├── MetaAdDashboard.pbix           # Main Power BI dashboard file
├── data/
│   ├── sample_campaign_data.csv   # Sample dataset
│   └── data_dictionary.md         # Column definitions
├── images/
│   ├── dashboard_screenshot.png   # Dashboard preview
│   └── insights_preview.png       # Key insights visualization
├── docs/
│   ├── DAX_measures.md            # DAX formulas documentation
│   ├── data_model.md              # Data model explanation
│   └── user_guide.pdf             # End-user guide
└── README.md                      # This file
```

---

## 📐 Sample DAX Measures

### Engagement Rate
```dax
Engagement Rate = 
DIVIDE(
    [Engagements],
   [Impressions],
    0
) * 100
```

### Click-Through Rate (CTR)
```dax
CTR = 
DIVIDE(
   [Clicks],
    [Impressions],
    0
) * 100
```

### Conversion Rate
```dax
Conversion Rate = 
DIVIDE(
   [Conversions],
    [Clicks],
    0
) * 100
```

For complete DAX documentation, see [docs/KPI](https://github.com/AdarshC10/POWER-BI/blob/main/Meta%20Ad%20Perfomance/Business%20Requirements%20Document_KPI.pdf)

---

## 🔮 Future Enhancements

- [ ] **Predictive Analytics:** Forecast campaign success using AI visuals
- [ ] **Advanced KPIs:** Add CPC (Cost Per Click) & CPA (Cost Per Acquisition)
- [ ] **Automated Alerts:** Notifications for unusual performance drops
- [ ] **Cross-Platform Comparison:** Compare Meta vs Google Ads vs LinkedIn Ads
- [ ] **Mobile Optimization:** Develop mobile-friendly dashboard layout
- [ ] **Real-Time Integration:** Connect directly to Meta Ads API
- [ ] **A/B Test Analysis:** Compare ad creative variants
- [ ] **Audience Insights:** Deep-dive into customer personas

---

## 🎓 Learning Outcomes

Through this project, the following skills were developed:

- ✅ Advanced Power BI visualizations and UX design principles
- ✅ Complex DAX formulas for marketing KPI calculations
- ✅ Star schema data modeling for optimal dashboard performance
- ✅ Social media marketing analytics and metrics interpretation
- ✅ Business storytelling through data visualization
- ✅ Understanding of digital marketing funnel metrics

---

## 📊 Use Cases

This dashboard is ideal for:

- 🎯 **Digital Marketing Teams** - Optimize campaign performance
- 💼 **Marketing Managers** - Monitor team KPIs and ROI
- 📈 **Growth Teams** - Identify scaling opportunities
- 💰 **Budget Planners** - Allocate resources effectively
- 🎓 **Students & Learners** - Study real-world marketing analytics

---

## 👤 Author

**Adarsh c**  
*Data Analyst | BI Developer | Marketing Analytics Specialist*

📧 Email: [adarshcrv@gmail.com](mailto:adarshcrv@gmail.com)  
💻 GitHub: [AdarshC10](https://github.com/AdarshC10)  


---


## 🙏 Acknowledgments

- Meta Business Suite for providing comprehensive campaign data
- Power BI community for visualization inspiration
- Digital marketing experts for metric validation
- Open-source contributors

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. 🍴 Fork the repository
2. 🌿 Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. ✍️ Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. 📤 Push to the branch (`git push origin feature/AmazingFeature`)
5. 🔀 Open a Pull Request

### Areas for Contribution
- Additional visualizations
- New DAX measures
- Documentation improvements
- Bug fixes and optimizations
- Sample datasets

---



<div align="center">

### 📊 Making Marketing Data Actionable

**Built with 💙 using Power BI**

[⬆ Back to Top](#-meta-ad-performance-dashboard)

</div>
