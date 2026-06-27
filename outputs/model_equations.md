# Model Equations

## Objective

The purpose of this analysis is to identify the factors that are most strongly associated with monthly sales performance across retail stores and provide evidence-based business recommendations.

---

# Simple Regression Models

## Simple Regression Model 1

### Equation

Monthly Sales = β₀ + β₁(Marketing Spend)

### Business Interpretation

This model examines whether stores that spend more on marketing tend to generate higher monthly sales.

A positive coefficient indicates that additional marketing investment is associated with increased sales.

---

## Simple Regression Model 2

### Equation

Monthly Sales = β₀ + β₂(Footfall)

### Business Interpretation

This model evaluates whether customer traffic is associated with store sales performance.

A positive coefficient indicates that stores with more customer visits generally achieve higher monthly sales.

---

# Multiple Regression Model

## Final Equation

```text
Monthly Sales =
394,161.94
+ 1.1145(Marketing Spend)
+ 29.3469(Footfall)
− 81,407.12(Avg Discount %)
+ 2,316.50(Staff Count)
+ 3,420.47(Region_North)
+ 12,266.09(Region_South)
```

---

# Model Performance

* Multiple R = 0.8882
* R² = 0.7890
* Adjusted R² = 0.7849
* Observations = 320

The model explains approximately **78.9% of the variation in monthly sales**, indicating strong explanatory power.

---

# Explanation of Each Coefficient

## Intercept = 394,161.94

The intercept represents the estimated monthly sales when all independent variables equal zero.

Although this situation is not realistic in practice, it provides the baseline level of sales used by the model.

---

## Marketing Spend Coefficient = 1.1145

### Direction of Relationship

Positive (+)

### Business Meaning

For every additional AED 1 spent on marketing, monthly sales are expected to increase by approximately AED 1.11, holding all other variables constant.

### Statistical Significance

* p-value = 2.66 × 10⁻¹⁴
* Statistically significant.

### Interpretation

Marketing investment is strongly associated with higher sales performance and should remain an important strategic focus.

---

## Footfall Coefficient = 29.3469

### Direction of Relationship

Positive (+)

### Business Meaning

Each additional customer visiting the store is associated with approximately AED 29.35 in additional monthly sales.

### Statistical Significance

* p-value = 5.13 × 10⁻²³
* Highly statistically significant.

### Interpretation

Footfall is one of the strongest predictors of monthly sales and should be a major management priority.

---

## Average Discount Percentage Coefficient = -81,407.12

### Direction of Relationship

Negative (-)

### Business Meaning

Higher discount levels are associated with lower monthly sales after controlling for other factors.

### Statistical Significance

* p-value = 0.044
* Statistically significant.

### Interpretation

The result suggests that aggressive discounting may reduce overall revenue and should be implemented carefully.

---

## Staff Count Coefficient = 2,316.50

### Direction of Relationship

Positive (+)

### Business Meaning

Adding one additional employee is associated with approximately AED 2,317 higher monthly sales.

### Statistical Significance

* p-value = 0.095
* Not statistically significant at the 5% level.

### Interpretation

The relationship is positive but relatively weak and should not be over-interpreted.

---

## Region_North Coefficient = 3,420.47

### Direction of Relationship

Positive (+)

### Business Meaning

Stores located in the North region generate approximately AED 3,420 more sales than stores in the reference category, all else being equal.

### Statistical Significance

* p-value = 0.623
* Not statistically significant.

### Interpretation

There is insufficient evidence to conclude that North region stores perform differently from the reference region.

---

## Region_South Coefficient = 12,266.09

### Direction of Relationship

Positive (+)

### Business Meaning

Stores in the South region generate approximately AED 12,266 more sales than stores in the reference category.

### Statistical Significance

* p-value = 0.089
* Not statistically significant at the 5% level.

### Interpretation

The positive relationship may be meaningful operationally but is not statistically strong enough to draw firm conclusions.

---

# Dummy Variable Approach

The categorical variable **Region** was converted into dummy variables.

## Reference Category

**East Region**

To avoid the Dummy Variable Trap (perfect multicollinearity), one category must be excluded from the model.

Therefore:

* East Region = Reference Category (not included in the regression equation)
* region_North = 1 if the store is located in the North region, otherwise 0.
* region_South = 1 if the store is located in the South region, otherwise 0.

The coefficients of the dummy variables measure the difference in monthly sales compared with stores located in the East region.

---

# Final Model Selected

## Multiple Regression Model

### Reason for Selection

The multiple regression model was selected because:

1. It has a high R² value of **78.9%**.
2. It incorporates several important business drivers simultaneously.
3. It provides better predictive power than the simple regression models.
4. It produces actionable business insights for management decision-making.

---

# Key Business Insights

The variables most strongly associated with monthly sales are:

1. Footfall
2. Marketing Spend
3. Average Discount Percentage (negative relationship)

Staff Count and Regional Variables appear relatively weak and should be interpreted cautiously.

---

# Important Note

Regression analysis demonstrates association rather than causation. The results should be used as evidence to support decision-making rather than proof that one variable directly causes changes in monthly sales.

