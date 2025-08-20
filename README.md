# Revenue Forecasting (Excel)

*Retail Sales & Revenue Forecasting in Excel*

Built an Excel model to forcast 2024 profit for a retail company under three sales growth scenarios. 
<br>

## 1. Business Problem
- Retail company needs to forecast sales, costs, and profit for next year.
- Management wants to know how different sales growth scenarios (best, base, worst) affect profit.

⭐️ Goal: Support strategic planning with data-driven insights.

<br>

## 2. Dataset
2023sales CSV file is [here](2023sales.csv)
- 12 months of historical sales & cost data from 2023.
- Variables include:
    - Sales by product category (Electronics, Clothing, Grocery).
    - Fixed Costs (rent, utilities, etc.).
    - Variable Costs (based on sales).
    - Staffing Costs (salaries, wages).
- Source: Dummy dataset created by me.

<br>

## 3. Excel Sheet '2023sales'
<img width="969" height="748" alt="스크린샷 2025-08-20 103347" src="https://github.com/user-attachments/assets/52edd3f8-69d5-4bb2-984f-c64cb48826ce" />

After opening the dataset in Excel, I added the following variables and row to the dataset:
- **Total Sales** using the SUM formula *of all sales*.
- **Total Costs** using the SUM formula *of all costs*.
- **Total Profit** using the profitability calculation *(Total Sales - Total Costs)*.
- **Year Total** using the SUM formula *of each column*.

I also added some visualizations that provide context to the original dataset.
- Bar Chart -> Total Sales by Month
- Pie Chart -> Sales share by Product Category

<br>

## 4. Scenario Sheet
<img width="730" height="169" alt="스크린샷 2025-08-20 103446" src="https://github.com/user-attachments/assets/8eec5208-128e-4de8-a3bc-4d47f4970387" />

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
<img width="654" height="317" alt="스크린샷 2025-08-20 103414" src="https://github.com/user-attachments/assets/af98ea27-2628-49fc-8407-fbfab6a42cb2" />

<br>

## 5. Results / Insights
-  Profit under the base case is expected to grow by 5%.
-  Every scenario highlights that Grocery Sales holds the biggest margin.
-  Worst-case scenario shows a big net loss.


⭐️ **Focus on scaling high-margin categories and prepare cost-control strategies in case of revenue decline.**

<br>

## 6. Access
Due to the Scenario Manager feature, the Excel sheet I attached [here](Revenue Analysis.xlsx) cannot open on Excel website. In order to interact with the Excel file, you must download the raw file and open through the Microsoft Excel app.
