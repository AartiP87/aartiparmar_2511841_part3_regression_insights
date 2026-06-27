# Model Comparison

## Objective

The purpose of this comparison is to evaluate the explanatory power and business usefulness of the simple and multiple regression models developed to understand the factors associated with monthly sales performance.

---

# Model Comparison Table

|                           |                        |                                                                                      |               |                        |                                            |                                                                                                                                                                              |                                                                                                                                                                                                      |
| ------------------------- | ---------------------- | ------------------------------------------------------------------------------------ | ------------- | ---------------------- | ------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                           |                        |                                                                                      |               |                        |                                            |                                                                                                                                                                              |                                                                                                                                                                                                      |
| **Model Name**            | **Dependent Variable** | **Independent Variables**                                                            | **R-squared** | **Adjusted R-squared** | **Significant Variables (p<0.05)**         | **Business Usefulness**                                                                                                                                                      | **Limitations**                                                                                                                                                                                      |
| Simple Regression Model 1 | monthly_sales          | marketing_spend                                                                      | 0.1672        | 0.1646                 | marketing_spend                            | Helps understand whether increasing marketing investment is associated with higher sales. Useful for evaluating advertising effectiveness and budgeting decisions.           | Ignores customer traffic, staffing, and regional differences. Low explanatory power because only one variable is included.                                                                           |
| Simple Regression Model 2 | monthly_sales          | footfall                                                                             | 0.7363        | 0.7355                 | footfall                                   | Demonstrates the importance of customer traffic in driving store sales. Useful for customer acquisition and store traffic strategies.                                        | Does not consider marketing activities, staffing, or regional effects. Cannot explain all variations in sales performance.                                                                           |
| Multiple Regression Model | monthly_sales          | marketing_spend, footfall, avg_discount_pct, staff_count, region_North, region_South | 0.7890        | 0.8046                 | marketing_spend, footfall,avg_discount_pct | Provides the most comprehensive explanation of sales performance by considering several business drivers simultaneously. Supports strategic decision-making and forecasting. | Regression shows association rather than causation. The model may omit important factors such as competition, seasonality, store management quality, economic conditions, and customer demographics. |

---

# Comparison of Explanatory Power

The simple regression models explain only a portion of the variation in monthly sales because they consider one predictor at a time.

The multiple regression model explains approximately **78.9%** of the variation in monthly sales, making it substantially more effective for understanding sales performance.

---

# Significant Variables

Based on the p-values from the multiple regression model:

### Statistically Significant Variables (p < 0.05)

* Marketing Spend
* Footfall
* Average Discount Percentage

### Variables That Are Statistically Weak (p > 0.05)

* Staff Count
* Region_North
* Region_South

Although these variables may have practical importance, there is insufficient statistical evidence to conclude that they have a strong relationship with monthly sales in this dataset.

---

# Business Usefulness of Each Model

## Simple Regression Model 1 – Marketing Spend

Useful for understanding whether marketing investment contributes to sales growth and for supporting advertising budget decisions.

---

## Simple Regression Model 2 – Footfall

Useful for understanding the importance of customer traffic and supporting initiatives that increase store visits.

---

## Multiple Regression Model

Provides the most useful business insights because it evaluates several factors simultaneously and controls for the effects of other variables. The model can be used to:

* Identify the strongest drivers of sales.
* Support resource allocation decisions.
* Prioritize marketing and customer acquisition strategies.
* Improve sales forecasting and performance monitoring.

---

# Limitations of the Models

The models do not capture several potentially important variables, including:

* Competitor activity
* Seasonality
* Economic conditions
* Customer demographics
* Store size
* Product assortment
* Store management quality
* Local market conditions

Additionally, regression analysis demonstrates statistical association and should not be interpreted as proof of cause-and-effect relationships.

---

# Final Model Selected

## Multiple Regression Model

### Reason for Selection

The multiple regression model was selected because:

1. It has the highest R-squared and Adjusted R-squared values.
2. It explains a large proportion of the variation in monthly sales.
3. It includes multiple business drivers simultaneously.
4. It provides the most actionable business insights for management decision-making.

---

# Conclusion

The analysis indicates that **footfall**, **marketing spend**, and **average discount percentage** are the variables most strongly associated with monthly sales performance. The multiple regression model provides the strongest explanatory power and should be used as the primary model for business decision-making and future sales analysis.
