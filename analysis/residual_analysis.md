# Residual Analysis

## Objective

Residual analysis was conducted to evaluate how well the final multiple regression model predicts monthly sales and to identify observations that are substantially under-predicted or over-predicted.

---

# Final Prediction Equation

Predicted Monthly Sales =

394,161.94

* 1.1145(Marketing Spend)
* 29.3469(Footfall)
  − 81,407.12(Avg Discount %)
* 2,316.50(Staff Count)
* 3,420.47(Region_North)
* 12,266.09(Region_South)

---

# Residual Formula

Residual = Actual Sales − Predicted Sales

Where:

* Positive Residual → Actual sales are higher than predicted.
* Negative Residual → Actual sales are lower than predicted.

---

# Calculating Predicted Sales in Excel

In the `Predictions_Residuals` sheet:

## Predicted Sales Formula

```excel
=394161.94
+(1.1145*Marketing_Spend)
+(29.3469*Footfall)
-(81407.12*Avg_Discount_Pct)
+(2316.50*Staff_Count)
+(3420.47*Region_North)
+(12266.09*Region_South)
```

## Residual Formula

```excel
=Actual_Sales - Predicted_Sales
```

---

# Largest Positive Residuals

Sort the Residual column from Largest to Smallest and record the five largest values.

|   |
| - |

| Rank      | Top 5 Positive Residuals |
| --------- | ------------------------ |
| Residuals |                          |
| 1         | 118256.0456              |
| 2         | 114844.5057              |
| 3         | 109808.3755              |
| 4         | 102538.4754              |
| 5         | 101096.831               |

## Business Interpretation

These stores generated substantially higher sales than predicted by the model.

Possible explanations include:

* Successful local marketing campaigns.
* Exceptional store management.
* Higher customer loyalty.
* Seasonal demand spikes.
* Local events or promotions.
* Strong product assortment.

The model is under-predicting these stores because important factors affecting performance are not included in the regression model.

---

# Largest Negative Residuals

Sort the Residual column from Smallest to Largest and record the five most negative values.

|   |
| - |

|   |
| - |

| Rank      | Top 5 Negative Residuals |
| --------- | ------------------------ |
| Residuals |                          |
| 1         | -138935.0426             |
| 2         | -126620.6286             |
| 3         | -126187.8242             |
| 4         | -123049.3765             |
| 5         | -122216.1136             |

## Business Interpretation

These stores generated substantially lower sales than predicted by the model.

Possible explanations include:

* Inventory shortages.
* Operational disruptions.
* Strong local competition.
* Poor customer experience.
* Store renovation or temporary closure.
* Economic challenges in the local market.

The model is over-predicting these stores because additional factors affecting sales performance are not captured in the dataset.

---

# Patterns Observed in Residuals

The residual analysis suggests that the model does not fully capture all factors affecting store performance.

Potential omitted variables include:

* Competitor activity
* Store size
* Customer demographics
* Economic conditions
* Seasonal effects
* Store management quality
* Product assortment differences

---

# Under-Predicted Stores

Stores with large positive residuals may represent:

* High-performing stores
* Stores with exceptionally strong customer loyalty
* Stores benefiting from temporary market opportunities

Management should investigate these stores to identify best practices that can be replicated across the retail network.

---

# Over-Predicted Stores

Stores with large negative residuals may represent:

* Underperforming stores
* Stores experiencing operational issues
* Stores facing strong competition

Management should investigate these stores to determine the causes of underperformance and implement corrective actions.

---

# Overall Conclusion

The residual analysis indicates that the multiple regression model performs well overall, explaining approximately **78.9%** of the variation in monthly sales.

However, some stores continue to experience prediction errors because important business drivers are not fully represented in the dataset.

Therefore, the model should be used as a decision-support tool rather than a perfect forecasting system.

Additional variables such as seasonality, competition, store size, and customer demographics may improve future model performance.
