#  Delivery Analysis Project 


## Overview

Delivr is a fictional food delivery startup created for practice purposes. This project is designed to help users enhance their SQL skills by working with a simulated real-world scenario. The dataset used in this project is sourced from DataCamp and serves as an educational tool to explore database management, querying, and analysis. 

Through the analysis, I analyzed weekly revenue and profit, profit for each meal, day of the week profit, retention rate and ARPU (average revenue per user) as KPIs to determine trends and performance. 
- [View code in Jupyter Notebook](https://github.com/kensuke0529/delivery_analysis/blob/main/csv_file/visualization.ipynb)

## Languages and Tools

- **SQL**: Data extraction and aggregation from relational databases.
- **Python**:
  - **Pandas**: Data transformation.
  - **Matplotlib/Seaborn**: Data visualization.
  - **Jupyter Notebook**: Interactive data analysis.

## Database Schema Overview

This project uses three main tables to manage Delivr's food delivery operations.

### 1. Meals
Stores basic information about the meals offered.

| Column Name   | Description                   |
|---------------|-------------------------------|
| `meal_id`     | Unique identifier for the meal |
| `meal_price`  | Selling price of the meal      |
| `meal_cost`   | Cost of producing the meal     |
| `eatery`      | Name of the restaurant offering the meal |


### 2. Orders
Manages user order data.

| Column Name       | Description                     |
|-------------------|---------------------------------|
| `order_id`        | Unique identifier for the order |
| `order_date`      | Date of the order               |
| `user_id`         | Unique identifier for the user  |
| `meal_id`         | Unique identifier for the meal ordered |
| `order_quantity`  | Quantity of the meal ordered    |

## Features

### 1. **Weekly Revenue and Profit Analysis**
- **Goal**: Measure weekly growth in sales and profit.
- **Key Insight**: Steady growth in both metrics, indicating a healthy market expansion.

![Weekly revenue](https://github.com/kensuke0529/delivery_analysis/blob/main/images/download.png)

#### Revenue increased by 3493% from May to December 2018. The highest growth happened in July with a 40.7% increase, followed by significant rises in September (28.5%) and October (26.8%). However, June and December decreased by -5.6% and -3.9%, respectively. Despite these declines, the overall trend was positive, reflecting strong growth throughout the period.

### 2. **Profit by each Meal**
- **Goal**: Identify the most and least profitable menu items.
- **Key Insight**: High-profit item can be promoted further, while low-margin items need improvement.

![Weekly revenue](https://github.com/kensuke0529/delivery_analysis/blob/main/images/profit.png)

#### Per-profit measures the profit per unit sold for each meal by dividing the total profit by the total quantity sold. Meal 11 has the highest per-profit of 4.75, which generates the most profit per item sold, while Meal 0 has the lowest per-profit of 2, indicating it generates the least profit per unit.


### 3. **Day-of-Week Profit Analysis**
- **Goal**: Evaluate whether the day of the week affects orders and profitability.
- **Key Insight**: Weekends show slightly higher performance, but no significant weekday trend.
![Weekly retention rate](https://github.com/kensuke0529/delivery_analysis/blob/main/images/output.png)

#### Wednesday was the least profitable day and Sunday was the most profitable, 24.7% more than Wednesday. Weekend profits were 11.8% higher than the weekday average.


### 4. **Retention Rate**
- **Goal**: Analyze weekly user retention to understand customer loyalty.
- **Key Insight**: Retention trends upward overall, with occasional dips requiring further investigation.
![Weekly retention rate](https://github.com/kensuke0529/delivery_analysis/blob/main/images/download%20(3).png)

#### From May to November 2018, the retention rate changed significantly on a weekly basis, with both increases and decreases. The highest weekly increase occurred from 08-06 to 08-13 (54.6%), while the largest decrease happened from 06-18 to 06-25 (-32.4%). The overall trend showed periods of growth, particularly in August, October, and November, with the retention rate improving significantly toward the end.

### 5. **ARPU (Average Revenue Per User)**
- **Goal**: Assess the average revenue generated per user each week.
- **Key Insight**: ARPU increases over time but shows seasonal fluctuations.
 
![Order nubmer](https://github.com/kensuke0529/delivery_analysis/blob/main/images/arpu.png)

#### The ARPU data shows steady overall growth of approximately 47.0%, starting at 22.7 and peaking at 33.7 in December. Seasonal trends are evident, with ARPU surging during November to December and dropping slightly during July (06-07 to 06-11) and early October (10-01 to 10-15). Weekly fluctuations indicate periodic highs and lows, but ARPU stabilized above 30.0 in late 2018.

## Future Improvements
- Expand the analysis to include external factors like marketing campaigns or weather data.

