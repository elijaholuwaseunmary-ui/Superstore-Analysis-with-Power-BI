**Power BI Superstore Sales Dashboard**

Project Overview

This project is an interactive Power BI dashboard built with theSuperstore Sales dataset. The goal was to transform raw sales data intomeaningful business insights that can support decisions around salesperformance, products, customers, profitability, and regionalperformance.

The dashboard uses interactive visuals, KPI cards, filters, Power Queryand DAX calculations to make the data easier to understand and analyze.

**Technologies Used**

1. Power BI Desktop

The main tool used to import, clean, model, analyze and visualize theSuperstore dataset.

2. Power Query

Used for data cleaning and transformation before the data was loadedinto the Power BI model.

Examples of transformations included: - Removing or handling errors andunnecessary values. - Checking and correcting data types. - Cleaningtext fields. - Splitting combined location information such as City andState where necessary. - Replacing invalid placeholder values such as-1 where appropriate. - Preparing date fields for analysis. - Ensuringnumerical fields such as Sales, Profit and Shipping Cost were storedcorrectly.

3. DAX (Data Analysis Expressions)

DAX was used to create calculated measures and support businessanalysis.

Examples include:

Total Sales = SUM(Superstore[Sales])

Total Profit = SUM(Superstore[Profit])

Total Orders = DISTINCTCOUNT(Superstore[Order ID])

Customer Purchased = DISTINCTCOUNT(Superstore[Customer ID])

Average Order Value = DIVIDE([Total Sales], [Total Orders])

Profit Margin = DIVIDE([Total Profit], [Total Sales])

Delivery Days =
DATEDIFF(
    Superstore[Order Date],
    Superstore[Ship Date],
    DAY
)

DAX made it possible to calculate KPIs dynamically as users interactwith the dashboard.

4. Data Visualization

Power BI visuals were used to communicate the results, including: -KPI/Card visuals - Line charts - Column charts - Bar charts - Donutcharts - Comparative charts - Slicers/filters

**Dashboard Features and Insights**

The dashboard provides an overview of the business through keyperformance indicators and visual analysis.

**Key Performance Indicators**

The dashboard displays: - Total Sales: approximately 14.90M -Total Profit: approximately 1.52M - Orders Processed:51 - Customers Purchased: 796 - Average Order Value:approximately 292.08K - Shipping Cost: approximately107.74K - Profit Margin: approximately 10%

These KPIs provide a quick summary of the overall business performance.

Sales Trend by Year

The yearly sales trend shows that sales were highest in 2009,declined through 2010 and 2011, and then increased again in2012.

This indicates that sales performance was not consistent across theyears and that the business experienced a recovery toward the end of theperiod.

Sales by Month

The monthly analysis shows differences in sales throughout the year.

The dashboard makes it possible to identify stronger and weaker salesmonths. December and January are among the stronger months, whileJune is one of the lower-performing months.

This insight can help with: - Seasonal sales planning - Marketingcampaigns - Inventory planning - Staffing and operational decisions

**Top Products by Sales**

The product analysis identifies products generating the highest sales.

Some of the leading products include products from the Zoom andXerox ranges.

This helps the business understand which products contribute most torevenue and which products may deserve stronger inventory and marketingattention.

Product Profitability

The profit analysis shows that high sales do not automatically mean highprofit.

Some products generate positive profit, while others generate very lowor negative profit. This is important because management should notfocus only on revenue; they should also consider the profitability ofindividual products.

Sales vs Profit

The comparison between Sales and Profit highlights the relationshipbetween revenue and profitability.

One of the important findings is that a product can have relativelyhigh sales without generating proportionally high profit. This canhappen because of discounts, costs, shipping expenses or other factors.

Order Priority

The donut chart shows the distribution of sales across order prioritiessuch as: - High - Low - Medium - Not Specified - Critical

This gives management an overview of how sales are distributed acrossdifferent order-priority categories.

**Project Process**

The project followed a typical data analytics workflow:

Step 1: Data Collection

The Superstore dataset was obtained and imported into Power BI.

Step 2: Data Understanding

The columns were reviewed to understand the structure of the dataset andidentify the fields needed for analysis.

Important fields included: - Order ID - Order Date - Ship Date -Customer ID - Customer Name - Product Name - Sales - Profit - ShippingCost - Order Priority - Location fields

Step 3: Data Cleaning

The data was prepared using Power Query.

The cleaning process included: 1. Checking for missing and invalidvalues. 2. Correcting data types. 3. Cleaning text values. 4. Splittingcombined fields where required. 5. Handling placeholder values such as-1. 6. Preparing date columns for time-based analysis. 7. Checkingnumerical columns for consistency. 8. Removing unnecessary data whereappropriate.

Step 4: Data Modeling

The cleaned data was loaded into the Power BI data model.

The model was structured so that measures and visualizations couldinteract correctly with the dataset.

Step 5: DAX Measures

DAX measures were created to calculate important business metrics suchas: - Total Sales - Total Profit - Total Orders - Customer Count -Average Order Value - Shipping Cost - Profit Margin - Delivery Days

Step 6: Dashboard Design

Visualizations were created based on the business questions.

The dashboard was designed using a green-themed color palette withKPI cards and charts arranged to make the information easy to read.

Step 7: Testing and Validation

The visuals and calculations were checked to make sure: - The numberswere reasonable. - Filters affected visuals correctly. - DAX measuresreturned the expected results. - Charts displayed the correct fields. -Titles and labels were understandable.

**File Structure**

A simple structure for the project is:

Power-BI-Superstore-Project/
│
├── README.md
│
├── Dataset/
│   └── Superstore Dataset
│
├── PowerBI/
│   └── Superstore Sales Dashboard.pbix
│
└── Screenshots/
    └── Dashboard screenshots

The .pbix file contains the Power BI data model, Power Querytransformations, DAX measures and dashboard pages.

**What I Learned**

This project helped me develop practical skills in data analytics andPower BI.

Data Cleaning

I learned that data cleaning is an important part of analytics becauseincorrect data types, missing values and invalid values can affect thefinal analysis.

**Power Query**

I learned how to transform raw data into a cleaner structure beforeanalysis.

**DAX**

I learned how to create measures using DAX and how functions such asSUM, DISTINCTCOUNT, DIVIDE, IF and DATEDIFF can be used toanswer business questions.

**Data Visualization**

I learned that choosing the correct visual is important. A line chart isuseful for trends, bar charts are useful for comparing products, and KPIcards are useful for displaying major performance indicators.

**Business Insight**

I learned that data analysis is not only about creating charts. The mostimportant part is being able to explain what the numbers mean and howthey can support business decisions.

**Problem Solving**

I also learned how to troubleshoot common Power BI issues such asincorrect data types, unexpected DAX results, visuals not displayingcorrectly and fields not behaving as expected.

**How the Project Can Be Improved**

Several improvements could make the dashboard more useful and professional.

1. Add More Interactivity

More slicers could be added for: - Year - Region - State - ProductCategory - Customer Segment - Order Priority

2. Improve the Data Model

A stronger star-schema model with separate dimension tables for Date,Customer, Product and Geography could improve performance andmaintainability.

3. Add More Profitability Analysis

The dashboard could include: - Profit by category - Profit by region -Profit by customer segment - Discount vs Profit - Products with highsales but negative profit

4. Add Forecasting

Sales forecasting could be added to estimate future sales based onhistorical trends.

5. Improve KPI Definitions

Some KPIs should be validated carefully against the dataset. Forexample, the dashboard should clearly distinguish between number oforders and number of order rows/transactions.

6. Improve Visual Design

The dashboard could be improved further with: - More consistentspacing - Clearer visual hierarchy - Shorter chart titles - Dynamictitles - Tooltips - Drill-through pages - Consistent number formatting

**Common Errors and Solutions**

Error 1: Incorrect Data Type

Problem: A number or date column is imported as text.

Solution: Open Power Query and change the column to the appropriatedata type, such as Whole Number, Decimal Number or Date.

Error 2: DAX Returning an Unexpected Result

Problem: A measure does not return the expected value.

Solution: - Check the column names. - Confirm the data type. - Checkthe filter context. - Make sure the correct measure is being used. - UseDIVIDE() instead of manually dividing where possible.

**Example:**

Average Order Value =
DIVIDE([Total Sales], [Total Orders])

Error 3: Visual Shows Only One Data Point

Problem: A scatter chart or other visual displays only one point.

Solution: Check whether a field that creates row-level detail has been added to the visual. Also check that the correct fields are placed in the X-axis, Y-axis and Details/Legend areas.

Error 4: Visual Cannot Load

Problem: Power BI displays an error such as an error fetching data for the visual.

Solution: - Check the fields used by the visual. - Check for invalid measures. - Refresh the data. - Check data types. - Remove and re-add problematic fields. - Recreate the visual if necessary.

Error 5: Text Values Affect Calculations

Problem: Numerical values are stored as text and cannot be calculated correctly.

Solution: Clean the values in Power Query and convert the column toa numerical data type.

Error 6: Incorrect Location Data

Problem: City and State information is combined in one field.

Solution: Use Power Query's Split Column feature to separate the information into appropriate fields.

Error 7: Date Analysis Not Working Correctly

Problem: Months appear in alphabetical order rather than chronological order.

Solution: Create a proper month number/date field and use Sort by Column so that January comes before February, February before March, and so on.

**Conclusion**

This Power BI project demonstrates how raw sales data can be transformed into an interactive business intelligence dashboard.

The project covers the complete analytics workflow:

Raw Data → Data Cleaning → Data Transformation → Data Modeling → DAX →Visualization → Business Insights

The main lesson from the project is that a good dashboard should not only look attractive; it should make complex data easier to understand and help users make better business decisions.

**Author**

Power BI Data Analytics Project

Built as part of my data analytics learning journey.
