Back to [Data Analytics Projects](<../../README.md>)
# **Diagnosing Sales Trends: Driving Factors & Customer Clustering**

**Goal:** Identify the key factors driving sales trends and determine which customer segments are most affected.<br>
**Function:** Perform diagnostic analytics to investigate the root cause of observed sales trends by analyzing historical sales data. Segment the client base according to their responsiveness to external factors.<br>
**Tools used:** MS Power BI, MS Excel<br>
**Features:** 
- Multi-metric analysis for trend cross-validation
- Data de-seasonalisation
- Macroeconomic impact analysis 
- Index-based comparative analysis
- Client segmentation with meaningful insights drawn from project-based segmentation
 

## Background

Initial decriptive company sales analysis revealed that while sales numbers appear strong in monetary value, sales volumes have been decreasing. This diagnostic study was launched to look into potential internal and external factors that could be driving this trend and identify the cause of the downward trend. 


## Diagnostic Analysis

**Sales volume trends measured by ticket volume**\
![](<1 Ticket volume.jpg>)

The graph analyzes only three quarters of data in a year to ensure comparability with the year 2023, for which fourth-quarter data is not yet available.

On the sales volume trend graph, three key features are observed: 

    - a downward trend since 2016, 
    - exceptionally low sales volume in 2020, and 
    - even lower in 2023. 

It is already known that the reason behind low activity in 2020 was the COVID-19 pandemic. The remaining two require further explanation.

Let's confirm that sales volumes have indeed been decreasing by using a different measure: tons instead of tickets. 

**Sales volume trends measured in tons**\
![](<2 Volume in tons.jpg>)

The issue is confirmed: the volume has been decreasing since 2016, and reached its lowest point in 2023. The study prioritizes tickets over tons wherever possible since data quality is superior with tickets.

Has the company been losing clients?

**Change in the Number of Active Clients per Year**\
![](<6 Active clients.jpg>)

On the contrary, the number of active clients per year has remained quite stable. Is the company losing long-term clients and replacing them with new ones?

**Sales Volume Trends of 30 Biggest Clients**\
![](<7 Activity of 30 biggest clients.jpg>)

The graph depicting the 30 biggest clients by purchase volume since 2015 assigns one client per color stripe. The graph provides 3 clues:<br>

    1) The company’s client base remained stable, with minimal turnover; however, existing clients experienced a reduction in their operations overall.<br>
    2) The shape of the graph indicates that the trends observed among its 30 largest clients closely mirror the company's overall trends.<br>
    3) The underlying cause of the decline appears to be widespread, impacting all clients across the board.
    
These clues point towards systemic causes: market forces or macroeconomic events.

The company's director was particularly interested in what happened in 2023. Let's identify when exactly in 2023 things started to go wrong by comparing monthly volume data in 2023 with other years.

**Tickets per Month**\
![](<3 Tickets per month.jpg>)

The volume graphs show strong seasonality due to industry-wide vacation periods in August and December. Let's adjust for seasonality to obtain a clearer view.

**Tickets per Month After Removing Seasonality Effects**\
![](<4 Deseasonalised tickets per month.jpg>)

The analysis confirms that the decline in sales throughout 2023 was not driven by isolated periods of underperformance but rather by a prolonged downturn throughout the year. Let's isolate the years 2022 and 2023 from the overall graph.

**De-seasonalized Sales Volumes Between January 2022 and October 2023**\
![](<5 Deseasonalised evolution of activity.jpg>)

This de-seasonalised graph shows that weak sales in 2023 did not stem from an acute problem in 2023: the decline began in 2022. The year 2022 began with strong performance but experienced a gradual decline throughout the year, which continued throughout 2023. To gain further insights, let's aggregate sales by quarter.

**Interest Rates**\
![](<8 Ticket volume v. interest rate.jpg>)

The blue column graph shows that the decline in sales, which severely affected 2023, started in the third quarter of 2022. Considering the slow and gradual impact that affected all the company's clients, macroeconomic factors should be examined.

On July 27, 2022, for the first time in 11 years, ECB raised the main refinancing rate from 0% to 0.5%. Subsequent interest rate hikes occured every few months (red line). 

The graph demonstrates an *inverse relationship* between quarterly sales volumes and the average ECB's interest rate for each quarter. 

**Inflation**\
![](<11 Activity to price index.png>)

But what about the gradual decline in sales volumes since 2016? If a price index provided by STATEC (in red), which was set to 100 in 2015, is plotted alongside the company's sales volumes on the graph as an index (in blue), an inverse relationship is observed: an increase in the price index generally coincides with a decrease in sales volumes. Since both curves are presented as indexes, it is evident that the decrease in sales volumes exceeds the increase in prices. These results are not surprising, given that the company operates in the discretionary spending sector.

This study concludes that the decline in sales volumes since 2016 was negatively influenced by an *increase in consumer prices*. and that the decline in sales volumes between the third quarter 2022 and the end of the studied period in October 2023 was negatively impacted by *rising interest rates*.


## Customer Clustering

Having identified the factors affecting sales performance, the next step is to group customers into meaningful segments based on their responsiveness to these factors.

To determine which customers were most affected by rising interest rates or contributed the most to the drop in sales volumes in 2023, sales volume in 2023 (right) is compared to the five-year average (2018-2022) sales volume (left). Only the first three quarters of data in each year are considered since fourth-quarter 2023 data is unavailable.

**Sales Volume by Client Project Sector in 2023 vs. Previous Five-Year Average**<br>
*(in nominal values)*\
![](<10 Volume by economic sector.jpg>)

Customers were grouped based on various characteristics available to the company, including headquarters location and legal structure. However, no significant differences in responsiveness were found among these groups.

In contrast, segmentation based on the nature of client projects proved more effective. If the reduction in the yellow area, representing projects of unknown type, is disregarded (as it signifies improved data collection in 2023), the most significant decrease in sales volume occurred in the bright green area, which represents projects by private individuals.

**Sales Volume by Client Sector in 2023 v. Previous Five-Year Average**<br>
*(as % of the total)*\
![](<9 Percentage of activity by economic sector.jpg>)

If the percentage of total sales volume contributed by each client project type is analyzed, all other project types gained importance in the total sales volume composition except for projects by private individuals.

Therefore, this study concludes that client projects ordered by *private individuals* were among most affected by rising interest rates.


## Improvement Opportunities

- Due to time constraints during the preparation of this report, the correlation between sales volumes and ECB interest rates, as well as the correlation between sales volumes and the consumer price index, was confirmed visually. An enhanced version of this study would incorporate correlation analysis to quantify relationships between variables and regression analysis to assess the impact magnitude of each factor.

- A more refined approach to customer clustering would be to first determine customer correlation coefficients for each key sales trend factor separately and then group customers based on their similarity in responsiveness to these factors.


Back to [Data Analytics Projects](<../../README.md>)
