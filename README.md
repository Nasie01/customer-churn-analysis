# Customer Churn Analysis

## Executive Summary

**Objective:**
The purpose of this analysis was to identify the key drivers of customer churn and assess their financial impact.

**Key findings:**
- The highest churn rate (28.1%) occurs within the first six months of product usage, while later tenure periods remain relatively stable at around 7–8%;
- Inactivity is a strong churn signal: churn increases steadily after 26 days without login (~20%) and exceeds 40% after 56 days; 
- Customers with low CSAT scores churn nearly three times more often than those with neutral or positive experiences;
  
**Non-significant factors:**
Age, usage growth rate, contract type, price increase, response time, and email open rate do not have a significant impact on churn, with differences across segments remaining within 1%.

**Financial impact:**
Customer churn results in revenue losses exceeding 860,000, with more than  670,000 coming from long-tenure customers.

**Recommendations:**
- Focus retention efforts on early risk signals, particularly low CSAT and prolonged inactivity;
- Prioritize retention of long-tenure users, as this segment represents the most stable and valuable revenue.

## Dataset

**Source:** [Customer Churn Prediction Business Dataset](https://www.kaggle.com/datasets/miadul/customer-churn-prediction-business-dataset)
Synthetic customer churn dataset with user behavior, activity, and billing features.

**Key Features:**
- Customer demographics (age, gender, location)
- Usage patterns and activity metrics
- Billing information and contract details
- CSAT scores and support interactions
- Tenure and engagement data

## Tools & Technologies

- **Python 3.9+**
- **Libraries:** pandas, matplotlib
- **Environment:** Jupyter Notebook

## Project Structure
```
customer-churn-analysis/
├── README.md                           # Project documentation
├── customer_churn.ipynb                # Main analysis notebook
├── churn_analysis_report.pdf           # Detailed findings report
├── visualizations/                     # Analysis visualizations
│   ├── Average Support Response Time by Churn.png
│   ├── Churn Increase After a Certain Period of User Inactivity.png
│   ├── Churn Rate (%) by Price Increase.png
│   ├── Churn Rate by Age Group.png
│   ├── Churn Rate by Complaint Type.png
│   ├── Churn Rate by Contract Type.png
│   ├── Churn Rate by Useg Growth Rate.png
│   ├── Churn by Tenure Segment.png
│   ├── Comparison of income by churn status.png
│   ├── Customer churn by csat group.png
│   ├── Revenue comparison - Customers who left vs. stayed (by contract).png
│   ├── Revenue comparison - Customers who left vs. stayed (by tenure).png
│   └── Users and Churn Rate by Email Open Rate Category.png
└── customer_churn.csv              # Dataset
```

## How to Run

### 1. Clone the repository:
```bash
git clone https://github.com/Nasie01/customer-churn-analysis.git
cd customer-churn-analysis
```

### 2. Install required packages:
```bash
pip install pandas matplotlib jupyter
```

### 3. Launch Jupyter Notebook:
```bash
jupyter notebook customer_churn.ipynb
```

### 4. Run all cells:
- Use **Cell → Run All** or press **Shift + Enter** to execute each cell

## Visualizations

The analysis includes comprehensive visualizations covering:

### Demographic & Behavioral Analysis:
- **Churn Rate by Age Group** - Age segmentation analysis
- **Churn by Tenure Segment** - Customer lifecycle patterns
- **Churn Rate by Contract Type** - Contract structure impact

### Engagement & Activity:
- **Churn Rate by Usage Growth Rate** - Usage pattern analysis
- **Churn Increase After User Inactivity** - Inactivity thresholds
- **Users and Churn Rate by Email Open Rate** - Engagement metrics

### Financial Impact:
- **Comparison of Income by Churn Status** - Overall revenue impact
- **Revenue Comparison by Contract Type** - Churned vs. retained customers
- **Revenue Comparison by Tenure** - Long-term vs. short-term customer value

### Customer Experience:
- **Customer Churn by CSAT Group** - Satisfaction score impact
- **Average Support Response Time by Churn** - Support quality analysis
- **Churn Rate by Complaint Type** - Issue type patterns
- **Churn Rate by Price Increase** - Pricing sensitivity

All visualizations are available in the `visualizations/` folder.

## Detailed Report

For comprehensive findings, insights, and business implications, see the [Analysis Report](analysis_report.pdf).

## Key Outcomes

- Clear identification of high-risk churn segments
- Revenue-critical user identification
- Actionable insights for retention strategies
- Data-driven recommendations for business decisions

## Research Questions

This analysis addresses the following questions:

1. Which age segments have higher churn and do they require a separate retention strategy?
2. How does churn change depending on the length of service usage (tenure)?
3. Which contract type has the highest churn and which has the lowest?
4. Is there a usage threshold after which churn drops?
5. Is there an increase in churn among customers who have not logged in for more than 14 days?
6. What is the financial impact of churn and which segments generate the most revenue loss?
7. How has churn changed among customers after the price increase compared to those who were not affected?
8. What types of support requests are associated with the highest churn?
9. How does average response time relate to churn? How does churn change with low CSAT?
10. Do customers with low email open rates have higher churn compared to others?

## 👤 Author

**Anastasiia** (Nasie01)
- GitHub: [@Nasie01](https://github.com/Nasie01)

*This project was created as part of a data analysis portfolio to demonstrate skills in exploratory data analysis, data visualization, and business insights generation.*
