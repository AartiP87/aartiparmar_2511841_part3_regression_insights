# Part 3: Regression-Based Business Insights & Model Interpretation

## Business Problem Summary

The objective of this project is to identify the factors associated with monthly sales performance across retail stores and provide recommendations to improve business performance.

## Dataset Description

The dataset contains monthly store-level information including:

* monthly_sales
* marketing_spend
* footfall
* avg_discount_pct
* staff_count
* region
* store_type

## Dependent Variable

* monthly_sales

## Independent Variables

* marketing_spend
* footfall
* avg_discount_pct
* staff_count
* region_North
* region_South

## Regression Approach

1. Data cleaning and preparation.
2. Creation of dummy variables.
3. Simple regression analysis.
4. Multiple regression analysis.
5. Residual analysis and model comparison.

## Dummy Variable Approach

The categorical variable region was converted into dummy variables.

Reference category:

* East Region

Dummy variables:

* region_North
* region_South

## Model Comparison Summary

The multiple regression model achieved the highest explanatory power and outperformed the simple regression models.

## Final Model Selected

Multiple Regression Model.

## Business Recommendation

Focus on increasing customer footfall, improving marketing effectiveness, and maintaining appropriate staffing levels.

## Assumptions and Limitations

Regression demonstrates association rather than causation. Important variables such as competition, economic conditions, and local market factors may not be fully captured.

## Screenshots Included

* simple_regression_output.png
* multiple_regression_output.png
* residuals_preview.png
* model_comparison_preview.png
