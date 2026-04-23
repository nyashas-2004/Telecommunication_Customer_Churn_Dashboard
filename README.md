# 📡 Telecommunication Customer Churn Dashboard

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Data Analysis](https://img.shields.io/badge/Data_Analysis-0078D4?style=for-the-badge&logo=powerbi&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

An interactive **Excel-based business intelligence dashboard** designed to analyze customer churn behavior across a telecommunications company operating in India. This project uncovers key drivers of churn, revenue trends, and customer segmentation patterns to support data-driven retention strategies.

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Dataset Description](#-dataset-description)
- [Dashboard Sheets](#-dashboard-sheets)
- [Key Metrics & Insights](#-key-metrics--insights)
- [Features](#-features)
- [How to Use](#-how-to-use)
- [Tools & Technologies](#-tools--technologies)
- [Folder Structure](#-folder-structure)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🔍 Project Overview

Customer churn is one of the most critical challenges in the telecom industry. This dashboard provides a **360-degree view of churn behavior** by analyzing customer demographics, service usage, contract types, and revenue contribution. The goal is to help business stakeholders identify at-risk customer segments and make informed decisions to improve retention.

**Business Questions Answered:**
- What percentage of customers are churning, and what is the revenue impact?
- Which contract types, payment methods, and internet services are associated with the highest churn?
- How does customer tenure affect the likelihood of churn?
- Which states and regions contribute most to churn?
- What are the revenue and charges patterns among churned vs. retained customers?

---

## 📊 Dataset Description

| Attribute         | Details                                      |
|-------------------|----------------------------------------------|
| **Source**        | Telecommunication CRM dataset                |
| **Records**       | 7,043 customers                              |
| **Features**      | 32 columns                                   |
| **Time Period**   | 2020 – 2026                                  |
| **Geography**     | 20 Indian states across 4 regions            |
| **Churn Rate**    | ~26.5% (1,869 churned / 5,174 retained)      |

### Column Reference

| Column | Description |
|--------|-------------|
| `customerID` | Unique identifier for each customer |
| `Start_Date` | Customer subscription start date |
| `Year`, `Month`, `Month_Name`, `Year_Month` | Time dimensions |
| `gender` | Customer gender (Male / Female) |
| `SeniorCitizen` | Whether the customer is a senior citizen (1 = Yes) |
| `Partner` | Whether the customer has a partner |
| `Dependents` | Whether the customer has dependents |
| `State`, `Region` | Geographic location |
| `Tenure` | Number of months with the company |
| `Tenure_Group` | Tenure bucket (New / Mid / Loyal) |
| `PhoneService`, `MultipleLines` | Phone service details |
| `InternetService` | Type of internet (Fiber optic / DSL / No) |
| `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport` | Add-on services |
| `StreamingTV`, `StreamingMovies` | Streaming services |
| `Contract` | Contract type (Month-to-month / One year / Two year) |
| `PaperlessBilling` | Whether the customer uses paperless billing |
| `PaymentMethod` | Payment method used |
| `MonthlyCharges` | Monthly billing amount |
| `TotalCharges`, `Revenue` | Cumulative charges and revenue |
| `Charges_Group` | Revenue tier (Low / Medium / High) |
| `Churn`, `Churn_Label` | Churn status (Yes/No and Churned/Retained) |

---

## 📂 Dashboard Sheets

| Sheet | Description |
|-------|-------------|
| `Telco_Dataset` | Raw cleaned dataset with 7,043 customer records |
| `Measures` | Calculated KPIs and DAX-style Excel measures |
| `Pivot_Table` | Aggregated pivot summaries used by the dashboard |
| `Dashboard` | Main interactive overview with KPIs and charts |
| `Customer` | Customer demographics and segmentation analysis |
| `Revenue` | Revenue breakdown and charges trend analysis |
| `Service` | Service adoption rates and their churn correlation |
| `Churn` | Deep-dive churn analysis by multiple dimensions |
| `Sheet1` | Supplementary working sheet |

---

## 📈 Key Metrics & Insights

### Churn Overview
- **Total Customers:** 7,043
- **Churned Customers:** 1,869 (~26.5%)
- **Retained Customers:** 5,174 (~73.5%)

### Contract Type & Churn
| Contract | Count | Churn Risk |
|----------|-------|------------|
| Month-to-month | 3,875 | High |
| One year | 1,473 | Medium |
| Two year | 1,695 | Low |

> 💡 Month-to-month customers are the highest churn risk segment.

### Internet Service & Churn
| Service | Count |
|---------|-------|
| Fiber optic | 3,096 |
| DSL | 2,421 |
| No internet | 1,526 |

### Payment Methods
| Payment Method | Count |
|----------------|-------|
| Electronic check | 2,365 |
| Mailed check | 1,612 |
| Bank transfer (automatic) | 1,544 |
| Credit card (automatic) | 1,522 |

### Geographic Coverage
- **20 Indian states** across **4 regions** (North, South, East, West, Central)
- Multi-year analysis from **2020 to 2026**

---

## ✨ Features

- ✅ **Interactive Dashboard** with slicers for dynamic filtering by year, region, and contract type
- ✅ **Customer Segmentation** by tenure group, demographics, and service usage
- ✅ **Revenue Analysis** with monthly and total charges breakdown
- ✅ **Churn Deep-Dive** across contract, payment method, internet service, and geography
- ✅ **KPI Cards** showing total customers, churn count, churn rate, and revenue at a glance
- ✅ **Pivot Tables** powering all visualizations for fast refresh and scalability
- ✅ **Color-Coded Visuals** for quick pattern recognition and executive reporting

---

## 🚀 How to Use

1. **Clone or download** this repository:
   ```bash
   https://github.com/nyashas-2004/Telecommunication_Customer_Churn_Dashboard.git
   ```

2. **Open** the file `telecommunication_churn_dashboard.xlsx` in **Microsoft Excel 2016 or later** (Excel 365 recommended for full slicer support).

3. **Navigate to the `Dashboard` sheet** for the main interactive overview.

4. **Use the slicers** (dropdowns/filters) to drill down by:
   - Year / Month
   - Region / State
   - Contract Type
   - Churn Status

5. **Explore individual sheets** (`Customer`, `Revenue`, `Service`, `Churn`) for deeper analysis on specific dimensions.

> ⚠️ **Note:** Enable macros and content if prompted by Excel for full interactivity.

---

## 🛠 Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Microsoft Excel** | Dashboard creation, pivot tables, charts |
| **Power Query** | Data transformation and cleaning |
| **Excel Pivot Tables** | Dynamic data aggregation |
| **Excel Slicers** | Interactive filtering |
| **Conditional Formatting** | Visual KPI indicators |

---

## 📁 Folder Structure

```
Telecommunication_customer_churn_dashboard/
│
├── telecommunication_churn_dashboard.xlsx   # Main Excel dashboard file
├── README.md                                # Project documentation
└── assets/                                  # Screenshots of dashboard
    ├── dashboard_overview.png
    ├── customer_analysis.png
    ├── revenue_breakdown.png
    ├── service_analysis.png
    └── churn_analysis.png
```

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve the dashboard, add new visualizations, or extend the dataset:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Yashas N**
- GitHub: [@nyashas-2004](https://github.com/nyashas-2004)
- LinkedIn: [@yashas-n04](https://www.linkedin.com/in/yashas-n04/)

---

> ⭐ If you found this project useful, consider giving it a star on GitHub!
