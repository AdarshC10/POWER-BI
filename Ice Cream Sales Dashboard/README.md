# 🍦 Ice Cream Sales Analysis Dashboard

[![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-yellow?logo=powerbi)](https://powerbi.microsoft.com/)
[![Excel](https://img.shields.io/badge/Excel-Data%20Source-green?logo=microsoftexcel)](https://www.microsoft.com/excel)
[![DAX](https://img.shields.io/badge/DAX-Analytics-blue)](https://dax.guide/)

A comprehensive Power BI analytical solution for evaluating ice cream sales performance across countries, product categories, and time periods. This dashboard transforms raw sales data into actionable business insights.

<img width="348" height="627" alt="image" src="https://github.com/user-attachments/assets/6dc11988-ee76-4759-9d0d-327882480e46" />


---

## 📊 Project Overview

The Ice Cream Sales Analysis Dashboard provides a holistic view of business metrics including:
- Total sales and revenue trends
- Order volume analysis
- Profit margins and performance
- Month-wise demand patterns
- Customer engagement metrics

This solution empowers stakeholders to identify best-selling products, understand buying patterns, and make data-driven strategic decisions.

---

## 🎯 Key Objectives

- ✅ Analyze total revenue and order trends across product categories and time periods
- ✅ Identify top-performing and under-performing ice cream products
- ✅ Understand customer buying patterns and monthly demand fluctuations
- ✅ Compare revenue share based on categories and sub-categories
- ✅ Provide decision-makers with a dynamic, interactive dashboard

---

## 🧠 Key Insights

From the dashboard analysis:

- **🏆 Top Performers:** Chocolate, Strawberry, and Butterscotch contribute the highest share of total sales
- **📈 Seasonal Trends:** Revenue peaks during mid-year months, indicating strong seasonal demand
- **👥 Customer Patterns:** Purchase trends closely correlate with month-on-month sales and profit
- **📊 Product Performance:** Vanilla and Mango show moderate performance compared to premium flavors
- **💰 Revenue Distribution:** Significant variation across product sub-categories

---

## 🛠️ Tools & Technologies

| Tool / Technology | Purpose |
|-------------------|---------|
| **Power BI Desktop** | Data visualization & dashboard development |
| **Excel / CSV** | Source dataset |
| **Power Query** | Data cleaning & transformation |
| **DAX** | KPI calculations & business logic |
| **Data Modeling** | Schema design & relationship optimization |

---

## ⚙️ Dashboard Features

### 📌 Key Performance Indicators
- Total Sales
- Total Orders
- Profit Margins
- YoY % Change
- Product Cost
- Customer Count

### 🎛️ Interactive Elements
- **Slicers** for filtering by Country, Year, Category, and Month
- **Donut Charts** showing revenue distribution by Category & Sub-Category
- **Waterfall Chart** revealing revenue change by Year and Product
- **Bar Charts** comparing Product-wise and Category-wise revenue
- **Line Charts** visualizing Monthly Sales and Monthly Profit trends
- Clean UI with smooth data exploration capabilities

---

## 🗂️ Data Model Structure

The dashboard uses a **Star Schema** for optimal performance:

```
Fact_Sales (Center)
├── Dim_Product    → Product Name, Category, Sub-Category
├── Dim_Date       → Year, Quarter, Month, Date
└── Dim_Country    → Country / Region information
```

**Fact Table:** `Fact_Sales`
- Transactional metrics: Sales, Orders, Profit, Cost, Customers

**Dimension Tables:**
- `Dim_Product` - Product details and categorization
- `Dim_Date` - Time intelligence
- `Dim_Country` - Geographic information

This star schema ensures efficient performance and flexible slicing across dimensions.

---

## 💼 Business Impact

This dashboard enables stakeholders to:

- 🔮 **Predict revenue patterns** and prepare for seasonal demand
- 📦 **Improve product stocking** and supply chain efficiency
- 🎯 **Identify high-value products** for targeted marketing campaigns
- 📉 **Reduce inventory wastage** by analyzing low-performing items
- 💡 **Improve customer engagement** through insight-driven decision-making

---

## 🚀 Getting Started

### Prerequisites
- Power BI Desktop (latest version)
- Sample dataset (Excel/CSV format)



---

## 📁 Project Structure

```
ice-cream-sales-dashboard/
│
├── IceCreamSalesDashboard.pbix    # Main Power BI file
├── data/
│   └── sales_data.csv              # Sample dataset
├── images/
│   └── dashboard_screenshot.png    # Dashboard preview
├── docs/
│   └── DAX_measures.md             # Documentation of DAX calculations
└── README.md                       # This file
```

---

## 🔮 Future Enhancements

- [ ] Add demand forecasting using Power BI AI visuals
- [ ] Integrate real-time data refresh via Power BI Service
- [ ] Implement geo-mapping to track outlet-level performance
- [ ] Add R/Python scripts for advanced predictive analytics
- [ ] Mobile-optimized layout for Power BI Mobile app

---

## 🎓 Learning Outcomes

Throughout this project, the following skills were developed:

- ✅ Designing star schema data models
- ✅ Building KPI-driven dashboards using Power BI
- ✅ Writing advanced DAX measures for analytics
- ✅ Performing data cleaning and transformation in Power Query
- ✅ Translating raw business data into meaningful insights

---

## 👩‍💻 Author

**Akshatha Reddy**  
*Data Analyst | Power BI Developer | Turning Data Into Insights*

📧 Email: [adarshcrv@gmail.com](mailto:adarshcrv@gmail.com)  
💻 GitHub: [@yourusername](https://github.com/AdarshC10)  


---



## 🙏 Acknowledgments

- Power BI community for inspiration and resources
- Sample dataset contributors
- Open-source visualization community

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📞 Contact & Support

If you have any questions or need support, feel free to reach out:

- 📧 Email: adarshcrv@gmail.com


---

<div align="center">

⭐ **If you found this project helpful, please consider giving it a star!** ⭐

Made with ❤️ and Power BI

</div>
