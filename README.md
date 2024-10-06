CREDIT CARD FINANCIAL DASHBOARD

Project Overview:

This project aims to develop a comprehensive credit card weekly dashboard that provides real-time insights into key performance metrics and trends. 
It enables stakeholders to effectively monitor and analyze credit card operations, offering critical data points for informed decision-making.
Key Features

    Real-time Data Analysis: Offers weekly insights into revenue, transactions, and customer demographics.
    Performance Metrics: Includes key metrics like total revenue, interest earned, transaction amounts, and customer count.
    DAX Queries: Utilizes powerful DAX functions to segment data by age groups, income levels, and calculate weekly revenue comparisons.

DAX Queries Highlights:

    Age Group Segmentation: Categorizes customers by age brackets for deeper insights.

    DAX

AgeGroup = SWITCH(
  TRUE(),
  'public cust_detail'[customer_age] < 30, "20-30",
  'public cust_detail'[customer_age] >= 30 && 'public cust_detail'[customer_age] < 40, "30-40",
  ...
)

Income Group Segmentation: Classifies customers into low, medium, and high-income groups.

DAX

    IncomeGroup = SWITCH(
      TRUE(),
      'public cust_detail'[income] < 35000, "Low",
      'public cust_detail'[income] >= 35000 && 'public cust_detail'[income] <70000, "Med",
      ...
    )

    Revenue Calculation: Summarizes key revenue components such as annual fees, transaction amounts, and interest earned.

Insights - Week 53 (31st Dec)

    Revenue Growth: Increased by 28.8% WoW
    Total Transaction: Increased by xx%
    Customer Count: Increased by xx%

Year-to-Date (YTD) Performance

    Overall Revenue: $57M
    Total Interest Earned: $8M
    Total Transaction Amount: $46M
    Top Customer Segments: Male customers contributed $31M, female customers $26M
    Top Credit Card Types: Blue & Silver cards account for 93% of all transactions
    Top Regions: Texas, New York, and California contributed 68% of the overall revenue
    Activation Rate: 57.5%
    Delinquency Rate: 6.06%

Conclusion:

This dashboard offers a detailed look into weekly and yearly performance metrics, 
making it an essential tool for stakeholders to track and optimize credit card operations efficiently.
