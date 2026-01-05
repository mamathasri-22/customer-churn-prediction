
# 🎯 Customer Churn Prediction - AI-Powered Banking Analytics

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0+-orange.svg)](https://scikit-learn.org/)
[![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow.svg)](https://powerbi.microsoft.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📋 Project Overview

An end-to-end machine learning project predicting customer churn in the banking sector with **86.5% accuracy**. Built by leveraging 1+ years of banking experience at Bank, this project identifies at-risk customers and provides actionable retention strategies.

### 🎯 Business Problem

Customer churn costs banks millions annually. This project analyzes customer behavior patterns to:
- **Predict** which customers are likely to churn
- **Identify** key churn drivers and risk factors
- **Recommend** targeted retention strategies
- **Quantify** potential revenue savings

### 💡 Key Achievements

- ✅ **86.5% prediction accuracy** using Random Forest Classifier
- ✅ Analyzed **10,000+ customer records** with 14+ features
- ✅ Identified **45% churn rate** in early customers (0-2 years)
- ✅ Built **interactive Power BI dashboard** for business insights
- ✅ Potential savings: **₹12.5 crores annually** (25% churn reduction target)

---

## 📊 Project Structure

```
customer-churn-prediction/
├── README.md
├── requirements.txt
├── .gitignore
├── LICENSE
│
├── data/
│   ├── raw/                                    # Original dataset
│   │   └── customer_churn_data.csv
│   └── processed/                              # Cleaned & segmented data
│       ├── customer_churn_cleaned.csv
│       ├── customer_churn_segmented.csv
│       ├── churn_powerbi_data.csv
│       └── model_performance_results.csv
│
├── notebooks/                                   # Jupyter notebooks
│   ├── 01_Customer_Churn_Exploration.ipynb    # EDA & cleaning
│   ├── 02_Advanced_Churn_Analysis.ipynb       # Segmentation & insights
│   └── 03_Churn_Prediction_Models.ipynb       # ML modeling
│
├── dashboards/
│   └── Customer_Churn_Dashboard.pbix          # Power BI dashboard
│
├── reports/
│   └── Customer_Churn_Analysis_Report.pdf     # Executive summary
│
└── images/                                      # Visualizations
    ├── churn_overview.png
    ├── model_comparison.png
    ├── confusion_matrix.png
    └── ...
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook / Google Colab
- Power BI Desktop (for dashboard)

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/mamathasri-22/customer-churn-prediction.git
cd customer-churn-prediction
```

2. **Install required packages**
```bash
pip install -r requirements.txt
```

3. **Launch Jupyter Notebook**
```bash
jupyter notebook
```

4. **Run notebooks in order:**
   - `01_Customer_Churn_Exploration.ipynb`
   - `02_Advanced_Churn_Analysis.ipynb`
   - `03_Churn_Prediction_Models.ipynb`

---

## 📊 Dataset Overview

**Source:** Banking customer data (Kaggle)  
**Records:** 10,000+ customers  
**Features:** 14 variables including:

| Feature | Description |
|---------|-------------|
| `CustomerId` | Unique customer identifier |
| `Geography` | Customer location (France, Germany, Spain) |
| `Gender` | Male/Female |
| `Age` | Customer age |
| `Tenure` | Years with bank |
| `Balance` | Account balance |
| `NumOfProducts` | Number of bank products used |
| `HasCrCard` | Credit card ownership (Yes/No) |
| `IsActiveMember` | Active/Inactive status |
| `EstimatedSalary` | Annual salary estimate |
| `Churn` | **Target variable** - Customer churned (Yes/No) |

---

## 🔍 Methodology

### 1. Data Exploration & Cleaning
- ✅ Loaded and inspected 10,000 records
- ✅ Handled missing values (none found)
- ✅ Analyzed distributions and outliers
- ✅ Visualized churn patterns across demographics

**Key Findings:**
- Overall churn rate: **20.4%**
- Customers aged 40-50 show the highest churn
- Geography: Germany has 32% churn vs France 16%

### 2. Advanced Analysis & Segmentation
- ✅ Created tenure segments (New, Growing, Mature, Loyal)
- ✅ Analyzed balance and salary distributions
- ✅ Identified high-risk customer profiles
- ✅ Calculated revenue at risk

**Insights:**
- New customers (0-2 years): **45% churn rate**
- Inactive members: **2.5x higher churn** than active
- High product complexity (3-4 products): **83% churn**

### 3. Machine Learning Modeling
Trained and compared 4 algorithms:

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-------|----------|-----------|--------|----------|---------|
| **Random Forest** | **86.5%** | **85.2%** | **87.8%** | **86.5%** | **92.1%** |
| Gradient Boosting | 85.3% | 84.1% | 86.5% | 85.3% | 91.5% |
| Logistic Regression | 81.2% | 79.5% | 82.7% | 81.1% | 88.3% |
| Decision Tree | 79.8% | 77.9% | 81.2% | 79.5% | 86.7% |

**Best Model:** Random Forest Classifier
- **86.5% accuracy** on test set
- Correctly identifies **87.8%** of churning customers
- **Top 5 Features:** Age, Number of Products, Geography, Active Member Status, Balance

### 4. Power BI Dashboard
Interactive dashboard with:
- 📊 Executive KPI cards (Total customers, Churn rate, Revenue at risk)
- 📈 Churn distribution by geography, gender, and age
- 🎯 Customer segmentation analysis
- 💰 Financial impact visualization
- 🔍 Detailed drill-down capabilities

---

## 💼 Business Impact & Recommendations

### 🎯 Strategic Recommendations

**1. Early Intervention Program (First 2 Years)**
- Dedicated relationship manager for new customers
- Welcome package with onboarding support
- Quarterly check-ins during the first 6 months
- **Expected Impact:** 20% reduction in early-stage churn

**2. Re-engagement Campaign (Inactive Members)**
- Gamification rewards for app usage
- Personalized offers based on transaction patterns
- Financial literacy workshops
- **Expected Impact:** 15% reactivation rate

**3. Product Simplification**
- Review product bundling strategy
- Reduce complexity for customers with 3+ products
- Clear value proposition communication
- **Expected Impact:** 30% reduction in product-related churn

**4. Predictive Intervention System**
- Deploy ML model in production
- Automated alerts for at-risk customers
- Proactive retention calls
- **Expected Impact:** Save 500-700 customers monthly

### 💰 Financial Projections

**Current State:**
- Churn Rate: 20.4%
- Churned Customers: 2,037 (of 10,000)
- Revenue at Risk: ₹50 crores

**With 25% Churn Reduction:**
- Customers Saved: 509
- Revenue Retained: ₹12.5 crores annually
- **ROI: 500%** (Implementation cost ₹2.5 crores)

---

## 🛠️ Technologies Used

### Programming & Data Analysis
- **Python 3.8+** - Core programming
- **Pandas** - Data manipulation
- **NumPy** - Numerical computing
- **Jupyter Notebook** - Interactive analysis

### Machine Learning
- **Scikit-learn** - ML algorithms & evaluation
- **Random Forest** - Best performing model
- **Gradient Boosting** - Ensemble method
- **StandardScaler** - Feature scaling

### Visualization
- **Matplotlib** - Statistical plots
- **Seaborn** - Advanced visualizations
- **Power BI** - Interactive dashboards

### Version Control
- **Git** - Version control
- **GitHub** - Code repository

---

## 📈 Key Visualizations

### Model Performance Comparison
![Model Comparison](images/model_comparison.png)

### Confusion Matrix - Random Forest
![Confusion Matrix](images/confusion_matrix.png)

### Feature Importance
![Feature Importance](images/feature_importance.png)

### Churn Analysis Dashboard
![Dashboard Page 1](images/dashboard_page1.png)

---

## 🎓 Skills Demonstrated

- ✅ **Exploratory Data Analysis (EDA)**
- ✅ **Data Cleaning & Preprocessing**
- ✅ **Feature Engineering**
- ✅ **Machine Learning Modeling**
- ✅ **Model Evaluation & Selection**
- ✅ **Business Intelligence (Power BI)**
- ✅ **Statistical Analysis**
- ✅ **Customer Segmentation**
- ✅ **Banking Domain Expertise**
- ✅ **Strategic Business Recommendations**

---

## 📝 Lessons Learned

1. **Domain Knowledge is Critical:** 1+ years banking experience helped identify meaningful customer segments
2. **Feature Engineering Matters:** Created tenure and balance segments that improved model performance
3. **Class Imbalance:** Addressed 80-20 split using stratified sampling
4. **Business Context:** Focused on recall over precision to catch more churners
5. **Actionable Insights:** Translated technical findings into business strategies with clear ROI

---

## 🔮 Future Enhancements

- [ ] Deploy model as REST API using Flask/FastAPI
- [ ] Implement real-time churn prediction pipeline
- [ ] Add customer lifetime value (CLV) analysis
- [ ] Integrate with CRM system for automated alerts
- [ ] A/B testing framework for retention strategies
- [ ] Deep learning models (Neural Networks) for comparison
- [ ] Time-series analysis for churn trend forecasting

---

## 👤 Author

**Mamathasri**  


- 💼 [LinkedIn]( linkedin.com/in/mamathasri-turukula-5055751aa)
- 🐙 [GitHub](https://github.com/mamathasri-22)
- 📧  turakalamamathasri@gmail.com

**Experience:**
- 1+ years in banking operations and customer analytics
- Expert in credit risk, customer retention, and business strategy
- Passionate about leveraging data science for business impact

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **ICICI Bank** - Domain expertise and business understanding
- **Kaggle Community** - Dataset and learning resources
- **Scikit-learn Team** - Excellent ML library
- **Power BI Community** - Dashboard best practices

---

## 📞 Contact & Feedback

Found this project helpful? Have suggestions for improvement?

- ⭐ **Star this repository** if you found it useful
- 🐛 **Report issues** via GitHub Issues
- 💬 **Connect on LinkedIn** for collaboration
- 📧 **Email me** for questions or opportunities

---

## 🎯 Related Projects

Check out my other data science projects:

1. [Banking Loan Approval Analysis](https://github.com/mamathasri-22/banking-loan-approval-analysis)
2. [Credit Risk Analysis](https://github.com/mamathasri-22/credit-risk-analysis)
3. [RSVP Movie Analysis](https://github.com/mamathasri-22/rsvp-movie-analysis)

---

### ⭐ If you found this project valuable, please star this repository!

**Last Updated:** January 2026
