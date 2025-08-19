# Revenue Forecasting (Excel)

*Retail Sales & Revenue Forecasting in Excel*

Built an Excel model to forcast 2024 profit for a retail company under three sales growth scenarios. 
<br>

## 1. Business Problem
- Retail company needs to forecast sales, costs, and profit for next year.
- Management wants to know how different sales growth scenarios (best, base, worst) affect profit.

⭐️ Goal: Support strategic planning with data-driven insights.

## 2. Dataset
- 12 months of historical sales & cost data from 2023.
- Variables include:
    - Sales by product category (Electronics, Clothing, Grocery).
    - Fixed Costs (rent, utilities, etc.).
    - Variable Costs (based on sales).
    - Staffing Costs (salaries, wages).
- Source: Dummy dataset created by me.

## 3. Excel Sheet '2023sales'
After opening the 2023sales [CSV file](2023sales.csv), I added the following variables and row to the dataset:
- **Total Sales** using the SUM formula *of all sales*.
- **Total Costs** using the SUM formula *of all costs*.
- **Total Profit** using the profitability calculation *(Total Sales - Total Costs)*.
- **Year Total** using the SUM formula *of each column*.

I also added some visualizations that provide context to the original dataset.
- Bar Chart -> Total Sales by Month
- Pie Chart -> Sales share by Product Category

## 4. Scenario Sheet
The Scenario Sheet is where I extracted the necessary data needed for utilizing the **Scenario Manager**.
Assuming Total Sales of Clothing is in cell B15 & growth rate is in cell F3, we insert the following formula:

**='2023sales'!B15 * (1 + $F$3)**


I applied this formula to the rest of the product categories and Total Costs. This formula ensures that every time our growth rate changes, our Sales & Costs change accordingly.

<br>
Finally, using Scenario Manager, we will create three different scenarios:

- Best Case Scenario: 10% sales growth.
- Base Case Scenario: 5% sales growth.
- Worst Case Scenario: -5% sales growth.

Our growth rate (cell F3) is going to be our changing cell. When we click 'Show', the chosen scenario's sales growth % will apply to the growth rate cell, impacting our whole sheet into the scenario selected.


 
## 4. Results / Insights
-  Profit under the base case is expected to grow by 5%.
-  Every scenario highlights that Grocery Sales holds the biggest margin.
-  Worst-case scenario shows a big net loss.


**Focus on scaling high-margin categories and prepare cost-control strategies in case of revenue decline.**
