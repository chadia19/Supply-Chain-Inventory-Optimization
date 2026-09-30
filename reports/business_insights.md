# Supply Chain Inventory Optimization — Business Insights

## 1. Executive Summary

## 2. Inventory Performance

## 3. Sales & Profitability

## 4. Demand & Forecasting

## 5. Supply Chain & Operations

## 6. Key Findings

## 7. Business Recommendations

## 8. Conclusion

## 2. Inventory Performance

The inventory analysis shows noticeable differences in inventory levels, coverage, and inventory value across the five warehouses.

### Inventory by Warehouse

| Warehouse | Avg. Inventory Level | Avg. Coverage Days | Total Inventory Value |
| --------- | -------------------: | -----------------: | --------------------: |
| WH_2      |               491.49 |              50.65 |        121,398,875.91 |
| WH_4      |               477.39 |              42.67 |        101,103,440.78 |
| WH_5      |               467.12 |              43.09 |        106,927,856.97 |
| WH_1      |               466.06 |              44.13 |         98,662,156.36 |
| WH_3      |               455.56 |              45.14 |         97,151,661.10 |

### Key Observations

* **WH_2 has the highest average inventory level**, at 491.49 units.
* WH_2 also has the **highest average inventory coverage**, at 50.65 days, indicating that its inventory represents a relatively large number of days of demand coverage.
* WH_2 has the **highest total inventory value**, at approximately 121.4 million.
* **WH_3 has the lowest average inventory level**, at 455.56 units, and the lowest total inventory value, at approximately 97.2 million.
* WH_4 has the lowest average inventory coverage among the five warehouses, at 42.67 days.
* The differences between warehouses suggest that inventory is not distributed uniformly across the network.

### Business Interpretation

The relatively high inventory coverage observed in WH_2 should be monitored alongside demand and sales performance. A high level of inventory coverage can provide protection against stockouts, but it can also indicate that capital is being tied up in inventory if demand does not justify the stock level.

The differences in inventory value between warehouses also provide an opportunity to investigate whether inventory allocation is aligned with actual demand and profitability.

### Recommendation

Inventory allocation should be reviewed at warehouse level by comparing:

* inventory levels,
* demand,
* inventory coverage,
* inventory value,
* and stockout risk.

This can help identify warehouses where inventory could potentially be rebalanced while maintaining an appropriate level of service.

### Inventory Risk Analysis

The inventory risk analysis shows that most records are classified as **Normal**, while a smaller portion falls below the defined reorder point.

| Inventory Status    |    Records |    Share |
| ------------------- | ---------: | -------: |
| Normal              |     86,463 |   94.76% |
| Below Reorder Point |      4,787 |    5.24% |
| **Total**           | **91,250** | **100%** |

### Key Observations

* **94.76%** of the records are classified as Normal.
* **4,787 records**, representing **5.24%** of the dataset, are below the reorder point.
* The proportion below the reorder point is consistent with the **5.25% Low Stock Rate** displayed in the Power BI dashboard.

### Business Interpretation

Although the majority of inventory records are within the normal range, the records below the reorder point represent situations where replenishment may need to be considered.

The analysis should be combined with demand, reorder gaps, supplier lead times, and inventory coverage to determine whether these cases represent temporary fluctuations or situations requiring operational action.

### Recommendation

The business should monitor items below the reorder point and prioritize the cases where low inventory is combined with:

* high demand,
* high demand forecast,
* long supplier lead time,
* or a significant reorder gap.

This can help prioritize replenishment decisions rather than treating every low-stock record in the same way.

## 3. Sales & Profitability

The analysis of sales and profitability shows a relatively balanced performance across the four regions.

### Revenue and Profit by Region

| Region | Total Revenue | Total Profit | Average Profit Margin |
| ------ | ------------: | -----------: | --------------------: |
| East   |  8,398,382.40 | 2,789,524.01 |                32.42% |
| North  |  8,411,171.01 | 2,788,397.27 |                32.33% |
| South  |  8,320,450.82 | 2,762,288.19 |                32.45% |
| West   |  8,296,332.99 | 2,747,991.76 |                32.34% |

The **East region** generated the highest total profit, with **2,789,524.01**, while the **North region** recorded the highest total revenue at **8,411,171.01**.

The differences between regions are relatively small. Total revenue ranges from approximately **8.30 million to 8.41 million**, while total profit ranges from approximately **2.75 million to 2.79 million**. This indicates that the overall business performance is relatively balanced across the four regions.

Profit margins are also very close, ranging from **32.33% in the North** to **32.45% in the South**. The South therefore has the highest average profit margin, although the difference compared with the other regions is small.

### Key Observation

The results do not show a major profitability imbalance between regions. The relatively similar revenue, profit, and profit-margin levels suggest that regional performance is generally consistent.

For further analysis, regional performance should therefore be examined together with **inventory levels, demand, promotions, and warehouse performance**. This can help identify whether differences in profitability are related to inventory management or operational factors rather than sales volume alone.


## 5. Supply Chain & Operations

The supply chain analysis focuses on supplier lead times, reorder gaps, order quantities, and reorder points across warehouses.

### Supply Chain Performance by Warehouse

| Warehouse | Average Supplier Lead Time (days) | Average Reorder Gap | Average Order Quantity | Average Reorder Point |
| --------- | --------------------------------: | ------------------: | ---------------------: | --------------------: |
| WH_4      |                              8.48 |              172.01 |                  19.28 |                305.38 |
| WH_2      |                              8.46 |              172.61 |                  19.32 |                318.88 |
| WH_3      |                              8.22 |              170.60 |                  19.22 |                284.96 |
| WH_1      |                              8.00 |              173.94 |                  19.24 |                292.12 |
| WH_5      |                              6.76 |              168.12 |                  19.30 |                299.00 |

WH_4 has the highest average supplier lead time at **8.48 days**, followed closely by WH_2 at **8.46 days**. In contrast, WH_5 has the lowest average supplier lead time at **6.76 days**.

The average reorder gap ranges from **168.12 in WH_5** to **173.94 in WH_1**. WH_1 therefore has the highest average reorder gap, while WH_5 has the lowest.

Average order quantities are very similar across all warehouses, ranging from **19.22 to 19.32 units**. This indicates that order quantities are relatively consistent between warehouses.

The average reorder point varies more noticeably. WH_2 has the highest average reorder point at **318.88**, while WH_3 has the lowest at **284.96**.

### Key Observation

The main operational difference between warehouses concerns **supplier lead time and reorder point levels**. WH_4 and WH_2 have the highest average supplier lead times, while WH_5 has a noticeably lower lead time.

These differences can be considered when evaluating inventory planning and replenishment policies. Warehouses with longer supplier lead times may require closer monitoring of inventory coverage and reorder points to reduce the risk of supply interruptions.

The relatively similar order quantities across warehouses suggest that differences in operational performance are not primarily explained by large variations in average order quantity.

## 6. Key Findings

The analysis of the supply chain dataset highlights several important findings:

1. **Inventory levels differ between warehouses.**
   WH_2 has the highest average inventory level at **491.49 units** and the highest average inventory coverage at **50.65 days**. WH_3 has the lowest average inventory level at **455.56 units**.

2. **Most inventory records are classified as Normal.**
   **86,463 records (94.76%)** are classified as Normal, while **4,787 records (5.24%)** are classified as Below Reorder Point.

3. **Below-reorder-point inventory has significantly lower coverage.**
   Records classified as Below Reorder Point have an average inventory coverage of only **15.96 days**, compared with **46.77 days** for Normal inventory.

4. **Demand is higher for records below the reorder point.**
   The average demand forecast is **24.57 units** for Below Reorder Point records, compared with **19.83 units** for Normal records. This indicates that lower inventory coverage is observed alongside higher forecasted demand.

5. **Regional sales and profitability are relatively balanced.**
   Total revenue ranges from approximately **8.30 million to 8.41 million**, while average profit margins remain close to **32%** across all regions.

6. **Forecasting performance is consistent across regions.**
   The average forecast error is **2.38** in all four regions, while the average demand gap remains close to zero.

7. **Supplier lead times vary between warehouses.**
   WH_4 has the highest average supplier lead time at **8.48 days**, while WH_5 has the lowest at **6.76 days**.

## 7. Business Recommendations

Based on the analysis, several actions can be considered to improve inventory and supply chain management:

### 7.1 Monitor Below-Reorder-Point Inventory

The **4,787 records** classified as Below Reorder Point should receive particular attention. Their average coverage is only **15.96 days**, while their average forecasted demand is higher than that of Normal records.

A practical approach would be to prioritize these cases according to demand, inventory coverage, supplier lead time, and reorder gap.

### 7.2 Improve Replenishment Monitoring

Warehouses with longer supplier lead times, particularly **WH_4 and WH_2**, can be monitored more closely when planning replenishment. Longer lead times may require earlier action to maintain sufficient inventory coverage.

### 7.3 Review Inventory Distribution Across Warehouses

The differences in inventory levels and inventory values between warehouses suggest that inventory is not distributed uniformly. Comparing inventory levels with demand, sales, and inventory risk can help identify opportunities for better allocation.

### 7.4 Continue Monitoring Forecast Accuracy

Although the average forecast error is consistent across regions, forecast performance should also be monitored by month, warehouse, and SKU. This can help identify specific situations where forecast deviations are larger than the regional average.

### 7.5 Use Power BI for Ongoing Monitoring

The Power BI dashboard can be used to monitor key indicators such as revenue, profit, inventory levels, inventory risk, coverage days, demand forecasts, reorder gaps, and supplier lead times.

## 8. Conclusion

This project demonstrates an end-to-end approach to supply chain and inventory analysis, starting with data preparation and feature engineering and continuing through PostgreSQL analysis and Power BI visualization.

The analysis shows that the overall business performance is relatively balanced across regions, while inventory and operational conditions vary between warehouses. In particular, records below the reorder point show substantially lower inventory coverage and higher forecasted demand.

These findings demonstrate how data analysis can support inventory monitoring, replenishment planning, demand forecasting, and operational decision-making. The combination of Python, PostgreSQL, SQL, and Power BI provides a complete workflow for transforming raw supply chain data into actionable business insights.
