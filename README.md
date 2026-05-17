# Customer Churn Analysis Dashboard

## Overview
This Power BI project analyzes customer churn patterns for a telecom company using customer demographics, usage behavior, and feedback data.  
The dashboard helps identify at-risk customers and supports data-driven retention strategies.

---

## Tools & Technologies
- Power BI
- Power Query
- DAX
- CSV

---

## Dataset Information

| Table | Description |
|---|---|
| Customers | Customer demographic and churn details |
| Usage | Call minutes, data usage, and messages |
| Feedback | Satisfaction scores and complaints |

---

## Key KPIs
- Total Customers
- Churned Customers
- Churn Rate
- Average Tenure
- Customer Satisfaction Score
- Total Complaints

---

## Dashboard Features
- Churn rate analysis
- Churn by age group, gender, and region
- Data usage vs churn analysis
- Satisfaction score distribution
- Complaints analysis
- Tenure-based churn analysis

---

## DAX Measures Used

### Total Customers
```DAX
Total Customers =
DISTINCTCOUNT(Customers[CustomerID])
```

### Churned Customers
```DAX
Churned Customers =
CALCULATE(
    COUNT(Customers[CustomerID]),
    Customers[Churn] = "Yes"
)
```

### Churn Rate
```DAX
Churn Rate =
DIVIDE([Churned Customers], [Total Customers], 0)
```

### Average Tenure
```DAX
Average Tenure =
AVERAGE(Customers[Tenure])
```

---

## Analytical Questions Solved
- What is the overall churn rate?
- Which age groups have the highest churn?
- How does data usage correlate with churn?
- What is the average tenure of churned customers?
- Which regions have the highest churn rate?
- What is the satisfaction score distribution?
- How many complaints were raised by churned customers?
- What is the churn rate by gender?
- Which usage patterns indicate potential churn?
- How does churn vary by tenure?

---

## Key Insights
- Customers with lower satisfaction scores showed higher churn.
- High complaint counts were linked to increased churn.
- Customers with shorter tenure were more likely to leave.
- Certain regions and age groups had higher churn rates.

---

## Dashboard Preview
(Add dashboard screenshot here)

---

## Conclusion
This dashboard provides insights into customer behavior and churn trends, helping businesses improve customer retention and reduce churn effectively.

---

## Author
### Pragyan Parimita Behera
