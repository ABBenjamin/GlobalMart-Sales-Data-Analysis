[METHODOLOGY for GlobalMart US Analysis with PowerQuery & Excel.xlsx]

Loaded the Global_Superstore.csv into PowerQuery.

Filtered for only complete records, i.e those with no null in Postal Code. This produces the entire US domestic dataset; confirmed by adjusting filter to produce different results (e.g. all results from US produces the same number of results as with non-null Postal Code).

Converted datatype of Order Date and Ship Date to datetime, using Use Locale English (United States) to avoid errors with MDY date format. Converted other columns to Currency or Whole Number where required.

Close & Load from PowerQuery.

Sorted data by Order Date

Created pivot tables of grouped sales/quantities/profit by region, product category & name, and Order Date.
Created pivot charts of each to provide clear visualisation of these.
Created line chart of Total Sales over time.
Created pivot table heatmap (using conditional formatting) of sales totals by region and category.

Calculated correlation between Discount and Profit columns.

FINDINGS:

Which Product Categories are the Most Profitable?

[SUMMARY]
Data show Office Supplies as the most valuable category in terms of total sales as well as total quantities sold, producing sales value of greater than Technology and Furniture combined, owing in part to a major spike in sales in December 2014. The Technology and Furniture categories generated similar totals, with Furniture coming slightly ahead in both total value and quantity sold, with technology lagging behind. This insight reveals the company's strengths and potential areas for improvement. Further analysis of sales patterns could help optimise product strategy and resource allocation, whilst accounting for potential outliers.

[SALES PERFORMANCE]
OFFICE SUPPLIES is the best-selling category by quantity, with 464 units sold, for a total value of $28,708.49. 
Mean unit sale value: $61.87.
Average profit per unit: $18.80. 
Mean sale value per order: $227.85.


FURNITURE follows with 130 units sold, for a total value of $13,321.21. 
Mean unit sale value: $102.47. 
Average profit per unit: $6.36.
Mean sale value per order: $370.03.

TECHNOLOGY follows with 107 units sold, for a total value of $12,505.38.
Mean unit sale value: $116.87.
Average profit per unit: $23.48. 
Mean sale value per order: $390.79.

[MARKET FOCUS]
The data suggest that, historically, Office Supplies is the strongest performing category, owing largely to the major sales spike in December 2014. However, the 2015 performance for each of the three categories is almost identical; this could be a sign of stabilising sales trends.
 
[POTENTIAL STRATEGIES]
The Sales Performance figures offers interesting insight: Office Sales, whilst dominant in terms of overall numbers, commands the lowest average price per unit. Technology, whilst lowest in quantity and overall sales value, commands the highest average price per unit, as well as the highest average profit per unit. These two points may be influenced or largely driven by outliers, however; Technology's higher average sale value per order might simply be due to the lower number of orders overall, just as Office Supplies' dominant performance is owed largely to the Q4 2014 spike, though with the small number of orders that make up the spike excluded, the category's overall total is still the greatest of the three at $14,460.58, though the lead is much reduced. 

 Potential strategies may include: 
1. Maintain focus across all three categories while monitoring whether the 2014 spike represents a genuine trend or a one-off event.

2. Focus on Office Supplies where the data indicates stronger overall sales volume and revenue contribution.

3. Investigate whether Technology can produce greater returns because of its higher value and profit per unit, while identifying why its quantity is comparatively low.


Are there any noticeable trends in sales over time?

[SUMMARY]
GlobalMart's sales show an overall upward trend from 2012 to 2016. A major spike in sales occurs in Q4 2014, reaching over 12000 in sales value. After mid-2014, sales become more volatile with higher peaks. Early performance shows stability below 2000 sales value monthly. Seasonal patterns may be apparent but appear inconsistent. Following the 2015 sales spike, sales values reach consistently higher, more variable rates than pre-2015, often exceeding 4000 monthly, though the spike itself is a clear outlier. 

[OVERALL INCREASING TREND]
There's a general upward trend in sales from 2012 to 2016, with sales peaks becoming higher over time.

[SIGNIFICANT SALES SPIKE]
Q4 2014 demonstrates the single greatest sales spike, reaching over 12,000 sales value.

[EARLY STABILITY]
From 2012 to mid-2014, sales were relatively stable, typically below 2000 sales value per month with an apparent seasonal spike in Q4.

[INCREASED VOLATILITY]
From Q3 2014, sales have remained higher and more volatile than in earlier years, frequently exceeding 4,000 sales value.

[POTENTIAL OUTLIER]
The extreme peak in earlier 2015 could be due to special events, marketing campaigns or promotions running at this point in time to explain the spike in sales, or a data anomaly, given how dramatically it stands out from the rest of the data.
The trends above suggest that GlobalMart has experienced significant growth and changes in its business between 2012 and 2016, with a particularly transformative event or change occurring around early 2015. The company may wish to investigate the factors behind the increased volatility and major sales spike to inform future strategies.


How do sales and profits vary by region?:

[SUMMARY]
Sales vary significantly across regions. Central US leads in Office Supplies (12,231 sales value), whilst Western US demonstrates a strong showing for Technology and Furniture, reaching approx. 6000 in sales for these categories. Eastern aand Central US show strong Office Supplies sales. Furniture sales are lowest in Central and Southern US (Approx 2000 sales value). Technology performs weakest in Eastern and Southern US. This regional variation suggests tailored strategies may be needed for each market to optimise sales performance; further exploration of market conditions (such as major competitors) may provide greater insight.

[INSIGHTS]
Sales vary significantly by region, with each region showing distinct product category strengths.

Office Supplies dominate in the Eastern and Central US regions, indicating strong demand for workplace essentials in these regions.

Western US performs well in Furniture and Technology sales, reaching approx 6000 in sales value each, suggesting a robust market for both home and office equipment.

Furniture sales are weakest in the Central and Southern US, with approx. 2000 in sales in each region.


Is there a correlation between discount and profit?
Yes, there is a weak negative correlation between Discount and Profit: -0.16. This means that whilst profit is lower when a discount is applied, across the dataset it is not significant enough to seriously affect profits; eliminating discounts would likely only lose goodwill with the customer.



[TOTALS]
$54,535.08 across all categories, breaking down into:
$28,708.49 for Office Supplies
$13,321.21 for Furniture
$12,505.38 for Technology


Average discount: 15%

Total Profit: $12,063.97

